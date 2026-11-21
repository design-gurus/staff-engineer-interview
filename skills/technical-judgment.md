# Technical Judgment Under Uncertainty

Technical judgment is the ability to make a sound decision before all the information is available. Staff interviewers test it by asking how you decided, not only what you decided. Four tools cover most of the questions: reversibility, the pre-mortem, debt as interest, and build or buy.

## Reversible and irreversible decisions

Amazon describes decisions as one-way doors and two-way doors. A two-way door can be reversed cheaply. A one-way door cannot.

| Decision | Cost to reverse | Door | Appropriate process |
|---|---|---|---|
| Name of an internal metric | Minutes | Two-way | Decide alone, today |
| Choice of a logging library | Days | Two-way | Decide within the team |
| Public API format | Every client must change | One-way | Written proposal and review |
| Primary database for 180 services | Quarters of migration | One-way | Document, alternatives, and a named decision owner |

The common error runs in both directions: weeks of review for a two-way door, and a hallway conversation for a one-way door. Match the speed and the number of reviewers to the cost of reversal.

## The pre-mortem

The pre-mortem is credited to Gary Klein. Before committing to a plan, the team imagines that the project has already failed and writes down the causes.

1. State the assumption: "It is one year later and the migration failed."
2. Each person lists causes independently for five minutes.
3. Rank the causes by likelihood and cost.
4. Change the plan for the top three.

For a scheduler migration, the top cause might be "the last five teams never migrate." The plan then changes: those five teams get migration help funded in advance, and the old scheduler receives a retirement date.

## Technical debt as interest

Technical debt is the future work created by choosing a quicker solution now. Treat it as a loan: the interest is the recurring cost, and the principal is the cost to fix it.

| Quantity | Example |
|---|---|
| Interest | Manual reruns of failed jobs take 6 engineer hours per week |
| Principal | Automating reruns takes 3 engineers for 4 weeks, about 480 hours |
| Payback period | 480 divided by 6 is 80 weeks |

A payback period of 80 weeks is weak when the system will be replaced in a year. If incidents double the interest to 12 hours per week, the payback falls to 40 weeks and the fix becomes reasonable. Some debt should be left unpaid, and a staff engineer can show the arithmetic.

## Build, buy, or adopt

Buying means paying a vendor. Adopting means using an open source project that your team must operate.

| Question | Why it matters |
|---|---|
| Who maintains it in year three? | The purchase price is small beside years of ownership |
| What does leaving cost? | Exit cost is the work needed to move away later |
| What happens if the vendor or the main author leaves? | A dependency without an owner becomes your work |
| Is this a difference customers notice? | Build what distinguishes the product; buy the rest |

## Estimating effort and risk

Give a range, not a single date: "8 to 14 weeks, and the range depends on how many job definitions need manual conversion." Compare the project with similar past projects, which is called a reference class. Keep a risk list in which each risk has an owner, and estimate again when a risk occurs.

## How this appears in the interview

- "Tell me about a decision you made with incomplete information."
- "When did you decide not to fix something?"
- "How did you decide between building and buying?"

A strong answer names the tool, shows the numbers, and states what would have changed the decision.

## Go deeper

- [Grokking Staff Engineer Interview](https://www.designgurus.io/course/grokking-staff-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=skills-technical-judgment) has a chapter on technical judgment, including estimating risk and the effect of AI coding tools on engineering quality.
- [Advanced System Design Fundamentals](https://www.designgurus.io/course/advanced-system-design-fundamentals?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=skills-technical-judgment) works through build versus buy and cost estimation with full arithmetic.
- [System design](../rounds/system-design.md) shows where the pre-mortem fits in a design round.
- Free article: [System design trade-offs: how to handle them as a senior engineer](https://www.designgurus.io/blog/complex-system-design-tradeoffs?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=skills-technical-judgment)
- Free answer: [Strategies for answering design trade-off questions](https://www.designgurus.io/answers/detail/what-are-the-strategies-for-answering-design-trade-off-questions?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=skills-technical-judgment)
