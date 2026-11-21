# Influence Without Authority

A staff engineer usually has no direct reports and cannot instruct another team to do anything. Influence without authority is the skill of getting a decision made and carried out by people who are free to refuse. It is the skill that behavioral interviewers at staff level ask about most.

## Four methods

| Method | What you do | Why it works |
|---|---|---|
| Map who must agree | List every team and person whose approval or work is needed | Nobody is surprised late in the process |
| Talk before the meeting | Meet each party alone and learn their objection | The meeting confirms a decision and does not start a debate |
| Agree on criteria first | Settle how the choice will be judged before discussing options | A disagreement about preferences becomes a comparison of facts |
| Name the decision owner | Identify one person who decides, and a date | A stalled discussion gains an end point |

## A worked example

A staff engineer proposes moving 26 teams from three job schedulers to one. Each team has a reason to decline.

1. **Map.** Three teams own the old schedulers. Twenty-three teams only run jobs on them. The director of platform owns the budget.
2. **Talk first.** Over two weeks, the engineer meets the three owning teams. One fears losing a feature that 40 jobs depend on. That feature is added to the goals.
3. **Criteria.** All three teams agree to judge options on missed runs, on-call pages, and migration days per team.
4. **Decision owner.** The director decides by a stated date, using a four-page document with two alternatives.

At the review meeting, no objection is new. The decision takes 30 minutes.

## Disagreeing with senior people

Disagree and commit is a practice in which a person states an objection clearly, and then fully supports the decision once it is made.

| Step | Example wording |
|---|---|
| Confirm the shared goal | "We both want fewer missed runs this quarter." |
| State the disagreement as a prediction | "I expect the patch to leave two of the six failure causes in place." |
| Propose a test or a review date | "Can we review the incident count in eight weeks?" |
| Commit | "I will support the patch and help ship it." |

Escalation means asking a shared manager to decide. It is appropriate when two parties have agreed on the facts and still cannot agree on the choice. Escalate together with the other party, in one message that presents both positions fairly.

## Saying no to a manager or product lead

A bare refusal ends the conversation. A refusal with costs and options continues it.

> "We can ship by the first of the month if the migration pauses for three weeks, which delays the retirement of the old scheduler by one quarter. Or we ship two weeks later and keep the migration on schedule. Which cost do you prefer?"

## Sponsoring and mentoring

Mentoring is giving advice. Sponsoring is giving an opportunity, such as handing the cutover plan to a senior engineer and staying available for review. Interviewers ask about both, and sponsorship is the stronger evidence of staff scope.

## How this appears in the interview

- "Tell me about a time you had to convince a team that did not report to you."
- "Describe a decision that was stuck. What did you do?"
- "Tell me about a time you disagreed with your manager."

In each answer, state who had to agree, what each party objected to, and what you changed in response. An answer in which nobody objected shows no influence.

## Common mistakes

- Presenting a proposal for the first time in a large meeting.
- Winning the argument and losing the working relationship.
- Escalating before the facts are agreed.
- Reporting that "everyone aligned" without saying how.

## Go deeper

- [Grokking Staff Engineer Interview](https://www.designgurus.io/course/grokking-staff-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=skills-influence-without-authority) has five lessons on influence, from building agreement across teams to driving a decision you do not own.
- [Grokking Modern Behavioral Interview](https://www.designgurus.io/course/grokking-behavioral-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=skills-influence-without-authority) covers conflict questions and answer structure.
- [Behavioral](../rounds/behavioral.md) shows how these stories are graded.
