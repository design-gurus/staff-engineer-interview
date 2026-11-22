# Technical Strategy and Design Docs

Most of a staff engineer's influence travels through writing. Three documents matter most: the design document, the architecture decision record, and the technical strategy. Interviewers ask about all three, and some companies set a written exercise as part of the loop.

## Three documents and when to use each

| Document | Purpose | Typical length | Use it when |
|---|---|---|---|
| Design document | Get a decision on how to build one system | 3 to 8 pages | The work takes more than a few weeks or affects another team |
| Architecture decision record (ADR) | Record one decision and its reasons | Half a page | The decision is made and future engineers will ask why |
| Technical strategy | Set direction for many decisions across teams | 2 to 5 pages | Teams keep making conflicting choices about the same problem |

## The design document

A design document exists to get a decision, not to collect comments. A structure that works:

1. **Problem.** Who is affected and a number for the cost.
2. **Goals and non-goals.** What the design will do and what it deliberately will not.
3. **Proposed design.** The approach in enough detail to review.
4. **Alternatives considered.** At least two, each with the reason for rejection.
5. **Cost and operational load.** Money per month and who is paged.
6. **Migration and rollback.** How the organization moves and how it returns.
7. **Decision requested.** Who decides and by what date.

Sections 4 and 7 are the ones most often missing. Without alternatives, reviewers propose their own. Without a named decision, the review ends with 64 comments and no outcome.

## The architecture decision record

The ADR format is credited to Michael Nygard. Each record has a title, the context, the decision, and the consequences. An example:

> **Title:** Use a durable queue for scheduler dispatch.
> **Context:** Six incidents last quarter came from jobs lost during restarts.
> **Decision:** Jobs are written to a durable queue before dispatch.
> **Consequences:** Dispatch latency rises by about 20 milliseconds. Jobs may run twice, so every job must be safe to repeat.

A durable queue stores each message on disk so that a restart does not lose it. ADRs stay useful after people leave because each one records the reasoning at the time of the decision.

## The technical strategy

Richard Rumelt, in *Good Strategy Bad Strategy*, describes a strategy as three parts: a diagnosis, a guiding policy, and coherent actions.

| Part | Meaning | Example |
|---|---|---|
| Diagnosis | A plain statement of the problem | "180 services use three messaging technologies, and each one needs its own on-call expertise" |
| Guiding policy | The rule that directs future choices | "New services use one technology; the other two accept no new producers" |
| Coherent actions | Specific steps that follow the policy | "Publish a client library, migrate the 12 highest-volume producers, set a retirement date" |

A list of goals without a diagnosis is not a strategy. "Improve reliability" directs no decision.

## How this appears in the interview

- **Behavioral:** "Tell me about a document you wrote that changed a decision."
- **System design:** the interviewer expects goals, non-goals, and alternatives stated as you would write them.
- **Written exercise:** a short strategy or design document completed at home in two to four hours.

For a written exercise, spend the first third of the time on the diagnosis. Reviewers commonly report that weak submissions propose actions for a problem they never defined.

## Running a design review

As the author, state which comments you need: blocking concerns first. As a reviewer, mark each comment as blocking or non-blocking. A blocking comment must be resolved before approval. End every review with a decision, an owner, and a date.

## Go deeper

- [Grokking Staff Engineer Interview](https://www.designgurus.io/course/grokking-staff-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=skills-technical-strategy-and-design-docs) has a chapter on design writing, including a complete written strategy built step by step.
- Lesson: [The Design Document](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/the-design-document?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=skills-technical-strategy-and-design-docs), in Grokking Staff Engineer Interview
- Lesson: [Architecture Decision Records](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/architecture-decision-records?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=skills-technical-strategy-and-design-docs), in Grokking Staff Engineer Interview
- Lesson: [Writing a Technical Strategy](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/writing-a-technical-strategy?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=skills-technical-strategy-and-design-docs), in Grokking Staff Engineer Interview
- [Advanced System Design Fundamentals](https://www.designgurus.io/course/advanced-system-design-fundamentals?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=skills-technical-strategy-and-design-docs) covers the cost and migration sections in depth.
- [System design](../rounds/system-design.md) shows the same structure used live in a 45-minute round.
