# The Staff Engineer Coding Interview

Most staff loops still include one coding round, and some include two. The round is commonly reported to be graded at senior level. A weak result can end the loop, but a strong result does not earn the staff level, because the level decision depends on the other rounds.

## What changes and what does not

| Aspect | Senior loop | Staff loop |
|---|---|---|
| Number of coding rounds | Usually 2 | Usually 1, sometimes 2 |
| Problem difficulty | Medium to hard | The same |
| Weight in the level decision | High | Low |
| Tolerance for messy code | Some | Less, because you are expected to set standards |

## What interviewers record

- You restated the problem and confirmed two or three edge cases before writing code.
- You named the approach and its time and space complexity before starting.
- The code is readable: clear names, small functions, and no dead branches.
- You tested the code by tracing an example, without being asked.
- You explained the trade-off when a faster and a simpler solution both existed.

Complexity here means how running time and memory grow as the input grows.

## Formats to expect

| Format | What it looks like | Preparation |
|---|---|---|
| Algorithmic problem | One or two problems in 45 minutes | Review the common coding patterns |
| Practical coding | Build a small component, such as a rate limiter or a cache | Practice writing complete, runnable classes |
| Code review | Read a change of about 100 lines and comment on it | Practice separating blocking issues from preferences |
| Debugging | Find a defect in unfamiliar code | Practice forming and testing one hypothesis at a time |

The code review and debugging formats are commonly reported to be more frequent at staff level than at senior level. A blocking issue is a problem that must be fixed before the change can merge.

## How much time to spend

Coding deserves about 15 percent of preparation time for an engineer who writes code every week. Raise that share to 30 percent if you have spent the last two years mostly on design and coordination.

A simple test decides it. Take three medium problems under a 25-minute limit each. If you finish two with correct, tested code, maintain the skill with three problems a week. If you finish one or none, coding needs daily practice until the test passes.

## A practical example

A common practical question is: "Implement a rate limiter that allows 100 requests per user per minute."

A staff-quality session covers four things in order:

1. Clarify the contract. Is the limit a fixed window or a sliding window? What happens to a rejected request?
2. Write a simple, correct version first, such as a sliding window log per user.
3. State its cost: one timestamp per request, so 100 entries per active user.
4. Describe the next step without building it: a token bucket to reduce memory, and shared storage when there are several servers.

A token bucket is a counter that refills at a fixed rate, and each request removes one token. Step four is where a staff candidate differs: the design discussion follows naturally from working code.

## Common failures

- Skipping practice because "staff engineers do not code in interviews."
- Writing code silently for 20 minutes.
- Starting with the optimized version and running out of time.
- Leaving no time to test.

## Go deeper

- [Grokking the Coding Interview](https://www.designgurus.io/course/grokking-the-coding-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=rounds-coding) teaches the coding patterns that cover most algorithmic problems.
- [Grokking Staff Engineer Interview](https://www.designgurus.io/course/grokking-staff-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=rounds-coding) covers the rounds that decide the level.
- See [the interview loop](interview-loop.md) for how the rounds combine.
