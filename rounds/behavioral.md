# The Staff Engineer Behavioral Interview

A staff behavioral round asks the same kinds of questions as a senior one, about conflict, failure, and ambiguity. The difference is in what a passing answer contains. A senior answer shows that you handled the situation well. A staff answer also shows the scope of the situation, the decision you made with its alternatives, and the effect on other teams.

## The three layers a staff answer adds

Most candidates use STAR, a structure that orders an answer as Situation, Task, Action, Result. STAR remains the base. A staff answer adds three layers to it.

| Layer | What to state | Example |
|---|---|---|
| Scope | How many teams, people, or systems were involved, and for how long | "26 teams owned jobs on the three schedulers" |
| The decision and its alternatives | What you chose, what you rejected, and why | "I proposed one shared scheduler instead of fixing each of the three" |
| Effect on other teams | What changed for people outside your team | "Each team spent about two days migrating, and on-call pages fell from nine a week to one" |

## Five question families

| Family | Typical question | What the interviewer listens for |
|---|---|---|
| Scope | "What is the largest technical problem you have owned?" | A problem nobody assigned to you |
| Ambiguity | "Tell me about a time the goal was unclear." | You defined the problem in measurable terms |
| Conflict | "Tell me about a disagreement with a senior engineer." | You agreed on criteria before arguing the answer |
| Failure | "Tell me about a decision you got wrong." | A real cost and a specific change afterward |
| Influence | "How did you get a team to adopt something they did not want?" | You learned their objection before the meeting |

## The same story at two levels

Question: "Tell me about a time you disagreed with a technical decision."

**Senior-level answer.** "My tech lead wanted a new database for our service. I thought our existing one was enough, so I ran a benchmark, showed the results, and we kept the existing database."

**Staff-level answer.** "Two teams wanted to adopt a new database, which would have been the fourth one our 45 teams operate. Before debating the choice, I asked both teams to agree on three criteria: on-call cost, migration effort, and query latency. On those criteria the existing database met the need with one schema change. One team still disagreed, so I wrote down their concern and a date to review it. Six months later, latency was within target and the review closed the question."

The second answer is longer by about 30 seconds. It adds the number of teams, the method of deciding, and what happened to the people who disagreed.

## Building a story bank

A story bank is a short list of prepared stories that together cover the common questions.

1. List six to eight projects or incidents from the last five years.
2. For each, write the scope, your decision, the alternatives, and the measured result.
3. Mark which of the five families each story can answer.
4. Check that every family has at least two stories.
5. Practice each story aloud until it takes under three minutes.

## Signals that lower the level

- Every story happens inside one team.
- The answer describes effort and not a decision.
- A conflict story ends with you being proven right and nothing else.
- A failure story has no cost.

## Go deeper

- [Grokking Staff Engineer Interview](https://www.designgurus.io/course/grokking-staff-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=rounds-behavioral) includes a staff behavioral question bank with weak and strong answers side by side for each family.
- [Grokking Modern Behavioral Interview](https://www.designgurus.io/course/grokking-behavioral-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=rounds-behavioral) teaches STAR, story banks, and company frameworks from the beginning.
- Interviewing at Amazon? See the free [Amazon Leadership Principles](https://github.com/design-gurus/amazon-leadership-principles) repository. More questions are in the [question bank](../cheat-sheets/question-bank.md).
