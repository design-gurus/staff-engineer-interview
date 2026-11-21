# Senior vs Staff Engineer

A staff engineer is not a faster senior engineer. Three things change between the levels: the scope of the problems, how long the decisions last, and how much of the work is done through other people. Interviewers look for evidence of all three, and years of experience are not evidence of any of them.

## The three differences

| Difference | Senior engineer | Staff engineer |
|---|---|---|
| Scope of problems | A problem inside one team or one service | A problem that crosses several teams and has no single owner |
| How long decisions last | Months; a wrong choice can be reworked in a sprint | Years; a wrong choice is expensive to reverse |
| Work through other people | Mostly your own code and reviews | Mostly documents, reviews, and decisions that other engineers carry out |

## One incident at two levels

A scheduled job that sends seller payouts runs twice on one night.

**A senior engineer** finds the cause in the team's scheduler, adds a check so that a job cannot start while its previous run is active, writes the incident report, and closes the ticket within a week. This is good senior work.

**A staff engineer** asks a wider question: how often does this happen across the company? The answer is six incidents last quarter, across three schedulers built by three teams, running 42,000 jobs a day for 26 teams. The staff engineer writes a problem statement, proposes one shared scheduler, gets the three owning teams to agree, and plans a migration that takes a year.

The technical skill in both responses is similar. The second response differs in scope (26 teams), in duration (a decision the company keeps for years), and in method (other engineers do most of the building).

## What does not change

- Staff engineers still need senior-level technical depth. Scope without depth fails the design round.
- Staff engineers still write code at most companies, although less of it.
- Staff is not a management role. A staff engineer usually has no direct reports.

## How each difference appears in the interview

| Difference | Round where it is tested | Typical question |
|---|---|---|
| Scope | [Behavioral](../rounds/behavioral.md) and [project deep dive](../rounds/project-deep-dive.md) | "What is the largest problem you have owned that nobody assigned to you?" |
| Decision lifetime | [System design](../rounds/system-design.md) | "How does this design change in three years?" |
| Work through others | [Behavioral](../rounds/behavioral.md) | "How did you get other teams to adopt it?" |

## A self-check

Answer each question with a specific example from the last two years.

1. Have you defined a problem that involved three or more teams?
2. Have you written a document that changed what another team built?
3. Have you made a technical decision that is still in place after two years?
4. Have you stopped or redirected a project that was going to fail?
5. Has an engineer taken on larger work because you gave them the opportunity?

Three or more specific answers suggest you have staff-level evidence to present. Fewer than three suggests gathering that evidence at work before interviewing, because an interview cannot create scope that did not exist.

## Common misreadings

- "Staff means the best coder on the team." The level measures the size of the problems, not the speed of the code.
- "Staff means ten years of experience." Committees grade evidence, and tenure is not on the form.
- "Staff means telling teams what to do." A staff engineer has no authority over other teams and must persuade them.

## Go deeper

- [Grokking Staff Engineer Interview](https://www.designgurus.io/course/grokking-staff-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=skills-senior-vs-staff) opens with a chapter on what a staff engineer does, including how to choose which problems to work on.
- [Staff archetypes](staff-archetypes.md) describes the four common forms of the role.
- [Levels](../cheat-sheets/levels.md) lists the commonly reported titles at large companies.
- Free article: [Staff engineer vs senior engineer: scope, expectations, and interview bar](https://www.designgurus.io/blog/staff-engineer-vs-senior-engineer?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=skills-senior-vs-staff)
- Free answer: [Why system design interview rounds matter for senior and staff engineers](https://www.designgurus.io/answers/detail/why-system-design-interview-rounds-matter-for-senior-and-staff-engineers?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=skills-senior-vs-staff)
