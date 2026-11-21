# The Staff Engineer System Design Interview

A senior design round asks for a system that works at the stated scale. A staff design round also asks what the real problem is, what the design deliberately leaves out, what it costs to run, and how the organization moves to it from the current system. The architecture diagram is about half of the answer.

## Senior design and staff design

| Topic | A senior answer | A staff answer adds |
|---|---|---|
| Requirements | Clarifies the stated question | Turns a vague complaint into a measurable problem statement |
| Scope | Lists features | Lists non-goals, each with a reason |
| Time | Designs for the stated scale | Plans year one and year three, with the trigger for each later stage |
| Cost | Estimates storage and traffic | Adds dollars per month and operational load on the owning team |
| Rollout | Describes the new system | Describes the migration from the old one, team by team |
| Risk | Lists failure modes | Runs a pre-mortem and changes the plan because of it |

A non-goal is something the design will not do, stated in advance so that nobody assumes it. Operational load is the recurring human work a system creates: pages, manual fixes, and upgrades. A pre-mortem is an exercise, credited to Gary Klein, in which the team imagines the project has already failed and lists the causes.

## The six decisions in one example

Suppose the question is: "Scheduled jobs keep failing. Fix it." Three schedulers, built by different teams, run 42,000 jobs a day for 26 teams.

1. **Problem statement.** "Six incidents last quarter came from missed or double runs. Success means zero missed runs and at most one page per week."
2. **Non-goals.** No workflow orchestration and no sub-second timing, because fewer than 2 percent of jobs need either.
3. **Evolution plan.** Year one is a single scheduler with at-least-once delivery. Multi-region execution starts only when a region outage costs more than a stated amount.
4. **Cost and load.** Compare one shared scheduler against three: machines per month, pages per week, and which team is paged.
5. **Migration.** Run old and new side by side, move the lowest-risk teams first, and define the exit criteria for turning each old scheduler off.
6. **Pre-mortem.** The most likely failure is a migration that stalls at 80 percent, so the plan funds the last 20 percent before work begins.

At-least-once delivery means every job runs one or more times, so each job must be safe to run twice.

## A 45-minute time budget

| Minutes | Activity |
|---|---|
| 0 to 8 | Problem statement, who is affected, success measure |
| 8 to 12 | Goals and non-goals |
| 12 to 27 | High-level design and the two hardest components |
| 27 to 35 | Cost, operational load, and the owning team |
| 35 to 42 | Migration and rollback |
| 42 to 45 | Risks and what you would revisit |

Interviewers rarely ask for the last three rows. A staff candidate reaches them without being asked.

## Signals interviewers record

- You asked who owns the current system before proposing a new one.
- You rejected at least one reasonable alternative and gave the reason.
- You stated a number for cost or load and used it to choose between two designs.
- You treated migration as part of the design.

## Go deeper

- [Grokking Staff Engineer Interview](https://www.designgurus.io/course/grokking-staff-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=rounds-system-design) teaches each of the six decisions as a lesson and combines them in one worked design.
- [Advanced System Design Interview, Volume II](https://www.designgurus.io/course/grokking-system-design-interview-ii?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=rounds-system-design) provides advanced case studies for practice.
- [Advanced System Design Fundamentals](https://www.designgurus.io/course/advanced-system-design-fundamentals?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=rounds-system-design) covers the mechanics of migrations and cost estimation. For core patterns, see the free [Grokking System Design](https://github.com/design-gurus/grokking-system-design) repository.
