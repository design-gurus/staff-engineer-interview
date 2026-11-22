# The Project Deep Dive Interview

The project deep dive is a 45 to 60 minute round about one project from your own history. Some companies call it a project retrospective. The interviewer asks you to explain the project and then questions your decisions until the limit of your knowledge is clear. It is the round that most often separates a staff offer from a senior offer.

## What the round measures

| Question in the interviewer's mind | Evidence that answers it |
|---|---|
| Was the scope at staff level? | Several teams were affected, and the work lasted quarters |
| Did the candidate decide, or only build? | You can name the alternatives and why each was rejected |
| Is the technical depth real? | You answer the third follow-up question as easily as the first |
| Does the candidate learn? | You describe a specific mistake and what changed afterward |

## Choosing the project

Score each candidate project from 0 to 2 on five criteria and choose the highest total.

| Criterion | 0 | 2 |
|---|---|---|
| Scope beyond your team | One team | Three or more teams |
| Decisions you made yourself | You implemented a plan | You chose the approach |
| A hard trade-off | The answer was obvious | Two good options, one given up |
| A measured result | "It went well" | A number, before and after |
| Something you would change | Nothing | A specific decision |

The most recent project is often the wrong choice. A project that ended a year ago has results you can measure.

## The order: context, constraints, choices, results

Explain the project in this order, in about eight minutes, before follow-up questions begin.

1. **Context.** The business problem, who was affected, and a number for the cost of doing nothing.
2. **Constraints.** Deadline, team size, systems you could not change, and who had to agree.
3. **Choices.** Two or three decisions, each with the alternative you rejected and the reason.
4. **Results.** The measured outcome, what went wrong, and what you would do differently.

A short example of the first two steps:

> "Search indexing took 9 hours, so new listings were invisible for most of a day. Sellers filed about 300 complaints a month. I had four engineers and two quarters, and the ranking team's query format could not change."

## Preparing for follow-up questions

Build a depth map: a table with one row per decision, prepared three levels deep.

| Level | Question to prepare | Example answer |
|---|---|---|
| 1 | What was the alternative? | A full rewrite on a streaming pipeline |
| 2 | What numbers supported the choice? | Incremental indexing reached 15 minutes at one third of the cost |
| 3 | What was the second-order effect? | The ranking team had to handle partial updates, which took them six weeks |

A second-order effect is a consequence of the decision that appears later or in another team.

## Discussing a mistake

Interviewers ask about mistakes in almost every deep dive. State four things: the decision, the information you had at the time, the cost, and what you changed afterward. "We underestimated launch traffic by a factor of three, search was degraded for 40 minutes, and capacity reviews now use the highest of three estimates" is a complete answer.

## Common failures

- Saying "we" for every decision, so the interviewer cannot tell what you did.
- Describing the architecture for 20 minutes and never reaching a decision.
- Choosing a project with one team and no disagreement.
- Having no numbers for the result.

## Go deeper

- [Grokking Staff Engineer Interview](https://www.designgurus.io/course/grokking-staff-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=rounds-project-deep-dive) has a five-lesson chapter on this round, including one project explained at weak, strong, and staff level side by side.
- Lesson: [Choosing the Project](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/choosing-the-project?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=rounds-project-deep-dive), in Grokking Staff Engineer Interview
- Lesson: [Context, Constraints, Choices, Results](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/context-constraints-choices-results?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=rounds-project-deep-dive), in Grokking Staff Engineer Interview
- Lesson: [Answering Detailed Questions About Your Project](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/answering-detailed-questions-about-your-project?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=rounds-project-deep-dive), in Grokking Staff Engineer Interview
- Managers face a similar round. See the [Engineering Manager Interview](https://github.com/design-gurus/engineering-manager-interview) repository and [Grokking the Engineering Manager Interview](https://www.designgurus.io/course/grokking-the-engineering-manager-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=rounds-project-deep-dive).
- Practice questions are in the [question bank](../cheat-sheets/question-bank.md).
