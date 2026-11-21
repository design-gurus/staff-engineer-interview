# Common Mistakes in Staff Engineer Interviews

Strong senior engineers fail staff loops for a small number of repeated reasons. Almost none of them concern technical skill. The ten mistakes below are ordered by the round where they appear, and each one has a specific fix.

## The ten mistakes

| # | Mistake | Round | Fix |
|---|---|---|---|
| 1 | Not confirming the target level | Recruiter call | Ask which level the loop is calibrated for |
| 2 | Solving the stated question without questioning it | System design | Write a measurable problem statement first |
| 3 | Listing no non-goals | System design | Name two things the design will not do, each with a reason |
| 4 | Stopping at the architecture | System design | Reserve the last ten minutes for cost, migration, and risk |
| 5 | Choosing a single-team project | Project deep dive | Choose a project that involved three or more teams |
| 6 | Saying "we" for every decision | Project deep dive | Say "I decided" for your decisions |
| 7 | Having no alternatives | Project deep dive | Prepare the rejected option for every decision |
| 8 | Stories without scope | Behavioral | Open with teams, duration, and a measured result |
| 9 | A failure story without a cost | Behavioral | State the cost in time, money, or incidents |
| 10 | Skipping coding practice | Coding | Take a timed test of three problems in week one |

## Three mistakes in detail

### Solving the stated question without questioning it

The interviewer says: "Design a faster deploy pipeline." A senior response begins with build caching. A staff response first asks what "faster" must achieve: "Deploys take two hours across 45 teams. Is the goal shorter waiting time for engineers, or more deploys per day?" The two goals lead to different designs. Interviewers at this level often write vague questions deliberately to see who notices.

### Saying "we" for every decision

"We decided to use incremental indexing" tells the interviewer nothing about you. Compare: "The team was split between a rewrite and incremental indexing. I proposed incremental indexing because it reached 15 minutes of delay at one third of the cost, and I wrote the comparison that the director approved." The second version gives the committee a sentence it can quote.

### A failure story without a cost

"We had some issues at launch, and we learned to test more" is a common answer and a weak one. A complete answer has four parts: the decision, the information available at the time, the cost, and the change afterward. "I sized capacity from average traffic, launch traffic was three times higher, search was degraded for 40 minutes, and reviews now use peak estimates" takes 15 seconds to say.

## Mistakes specific to experienced candidates

- **Answering from your current system.** You describe how your company built it, and the interviewer's constraints are different. Design for the question asked.
- **Silent competence.** You make good decisions and do not say them aloud. Feedback forms record only what was spoken.
- **Over-engineering from past incidents.** You add protection against every failure you have seen. State the risk, estimate its cost, and include the protection only when the cost justifies it.
- **Relying on the title.** A current staff title is not evidence. The committee grades the stories.

## A check before the onsite

Answer yes or no.

1. Has the recruiter confirmed the target level?
2. Does every story open with scope?
3. Can you name the rejected alternative for each decision in your project?
4. Does your failure story include a cost?
5. Have you completed a design that reached migration and cost within 45 minutes?
6. Have you solved two of three medium coding problems in 25 minutes each?

Any "no" identifies the next hour of preparation.

## Go deeper

- [Grokking Staff Engineer Interview](https://www.designgurus.io/course/grokking-staff-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=cheat-sheets-common-mistakes) shows weak, strong, and staff-level answers side by side, so each of these mistakes is visible in a real answer.
- [Grokking Modern Behavioral Interview](https://www.designgurus.io/course/grokking-behavioral-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=cheat-sheets-common-mistakes) covers answer structure for failure and conflict questions.
- Next: the [four-week plan](four-week-plan.md) and [down-leveling](down-leveling.md).
