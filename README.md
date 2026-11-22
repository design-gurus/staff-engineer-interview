# Staff Engineer Interview

> The free, open companion to **Grokking Staff Engineer Interview** by [DesignGurus.io](https://www.designgurus.io/course/grokking-staff-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme), created by Arslan Ahmad.

[![GitHub stars](https://img.shields.io/github/stars/design-gurus/staff-engineer-interview?style=social)](https://github.com/design-gurus/staff-engineer-interview/stargazers)
[![Last commit](https://img.shields.io/github/last-commit/design-gurus/staff-engineer-interview)](https://github.com/design-gurus/staff-engineer-interview/commits/main)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](LICENSE)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

A senior engineer interview asks whether you can build the right system. A staff engineer interview asks whether you can choose the right problem, get several teams to agree on a design, and make decisions that still hold three years later. The rounds have familiar names, but the evidence that each round collects is different.

This repository is a short, free guide to that difference. It covers each round, the skills the rounds measure, and a set of cheat sheets for the final weeks of preparation. Each page takes about three minutes to read. For full lessons, worked answers, and mock loops, see the course.

## Start here

| Your situation | Read this first |
|---|---|
| You are a senior engineer and want to know what staff level means | [Senior vs staff engineer](skills/senior-vs-staff.md) |
| You have a staff loop scheduled and need the outline | [The interview loop](rounds/interview-loop.md) |
| You have four weeks to prepare | [Four-week plan](cheat-sheets/four-week-plan.md) |
| You want practice questions | [Question bank](cheat-sheets/question-bank.md) |
| You received a senior offer after a staff loop | [Down-leveling](cheat-sheets/down-leveling.md) |

## The loop at a glance

Most staff loops are commonly reported to contain four or five rounds of 45 to 60 minutes each. The exact set varies by company and by team.

| Round | What it measures at staff level | Guide |
|---|---|---|
| System design | Problem framing, non-goals, cost, migration, and a plan that changes over time | [System design](rounds/system-design.md) |
| Project deep dive | Whether you made the hard decisions in a large project, and how well you can defend them | [Project deep dive](rounds/project-deep-dive.md) |
| Behavioral | Scope, influence across teams, conflict with senior people, and failure | [Behavioral](rounds/behavioral.md) |
| Coding | Clean, correct code at senior level; rarely the deciding round | [Coding](rounds/coding.md) |

## All pages

### Rounds

| Page | What it covers |
|---|---|
| [The interview loop](rounds/interview-loop.md) | Every stage from recruiter call to hiring committee, and the evidence each one produces |
| [System design](rounds/system-design.md) | The six decisions that separate a staff design from a senior design |
| [Project deep dive](rounds/project-deep-dive.md) | How to choose a project and explain it as context, constraints, choices, results |
| [Behavioral](rounds/behavioral.md) | The three layers a staff answer adds to a standard behavioral answer |
| [Coding](rounds/coding.md) | What the coding bar is at staff level and how much time to spend on it |

### Skills

| Page | What it covers |
|---|---|
| [Senior vs staff engineer](skills/senior-vs-staff.md) | The three differences: scope, decision lifetime, and work done through other people |
| [Staff archetypes](skills/staff-archetypes.md) | Tech Lead, Architect, Solver, and Right Hand, and how each one interviews |
| [Technical strategy and design docs](skills/technical-strategy-and-design-docs.md) | Design documents, architecture decision records, and a written strategy |
| [Influence without authority](skills/influence-without-authority.md) | Building agreement across teams that do not report to you |
| [Technical judgment](skills/technical-judgment.md) | Reversible decisions, pre-mortems, technical debt, and build or buy |

### Cheat sheets

| Page | What it covers |
|---|---|
| [Question bank](cheat-sheets/question-bank.md) | About 50 staff interview questions in seven groups |
| [Levels](cheat-sheets/levels.md) | Commonly reported staff titles at Google, Meta, and Amazon |
| [Down-leveling](cheat-sheets/down-leveling.md) | Why it happens, how to see it coming, and what to do |
| [Four-week plan](cheat-sheets/four-week-plan.md) | A week-by-week preparation schedule with a finish condition for each week |
| [Common mistakes](cheat-sheets/common-mistakes.md) | Ten mistakes that strong senior engineers make in staff loops |

## FAQ

### What is a staff engineer interview?

A staff engineer interview is a hiring loop for the level above senior engineer on the individual contributor track. It usually contains a system design round, a project deep dive, one or two behavioral rounds, and a coding round. The loop tests whether a candidate can lead technical work across several teams without managing them. See [the interview loop](rounds/interview-loop.md).

### How is a staff engineer interview different from a senior engineer interview?

The round names are mostly the same, and the grading is different. A senior loop grades the quality of your solution. A staff loop also grades how you chose the problem, which alternatives you rejected, and how the decision affected other teams. See [senior vs staff engineer](skills/senior-vs-staff.md).

### What questions are asked in a staff engineer interview?

Expect open design questions with vague requirements, a 45-minute discussion of one project you led, and behavioral questions about scope, ambiguity, conflict, failure, and influence. The [question bank](cheat-sheets/question-bank.md) lists about 50 of them.

### How long does it take to prepare for a staff engineer interview?

Four weeks at 8 to 10 hours per week is a reasonable plan for an engineer who already works at senior level. Most of that time goes to the project deep dive and the behavioral stories, because that material cannot be studied from a book. See the [four-week plan](cheat-sheets/four-week-plan.md).

### What is down-leveling?

Down-leveling is an offer one level below the level you interviewed for, such as a senior offer after a staff loop. It usually means the loop found senior-quality work without enough evidence of staff scope. See [down-leveling](cheat-sheets/down-leveling.md).

### Do staff engineers still have a coding interview?

Yes, at most companies. The coding round is commonly reported to be graded at senior level, so it can fail a candidate but rarely earns the staff level alone. See [coding](rounds/coding.md).

## Course lessons to start with

- [Senior and Staff Engineers](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/senior-and-staff-engineers?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): how the two levels differ in scope and judgment, in Grokking Staff Engineer Interview
- [The Four Staff Archetypes](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/the-four-staff-archetypes?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): the four common forms of the staff role, in Grokking Staff Engineer Interview
- [From a Vague Ask to a Problem Statement](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/from-a-vague-ask-to-a-problem-statement?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): how to open a staff system design round, in Grokking Staff Engineer Interview
- [Worked Design: Consolidating Three Job Schedulers](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/worked-design-consolidating-three-job-schedulers?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): one complete staff-level design, in Grokking Staff Engineer Interview
- [Context, Constraints, Choices, Results](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/context-constraints-choices-results?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): the order for presenting a project in the deep dive, in Grokking Staff Engineer Interview
- [Writing a Technical Strategy](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/writing-a-technical-strategy?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): the parts of a written strategy, in Grokking Staff Engineer Interview
- [Building Agreement Across Teams](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/building-agreement-across-teams?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): how to move a decision across teams without authority, in Grokking Staff Engineer Interview
- [What a Staff Answer Adds](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/what-a-staff-answer-adds?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): what separates a staff behavioral answer from a senior one, in Grokking Staff Engineer Interview
- [Down Leveling: Causes and Responses](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/down-leveling-causes-and-responses?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): why a lower offer happens and how to respond, in Grokking Staff Engineer Interview
- [Running the 45 Minutes](https://www.designgurus.io/course-play/advanced-system-design-fundamentals/doc/running-the-45-minutes?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): how to divide the time in a design round, in Advanced System Design Fundamentals

## Free reading on DesignGurus.io

- Free article: [The staff engineer interview](https://www.designgurus.io/blog/staff-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): what changes from senior, round by round.
- Free article: [Staff engineer vs senior engineer](https://www.designgurus.io/blog/staff-engineer-vs-senior-engineer?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): scope, expectations, and the interview bar.
- Free article: [Staff engineer levels at Google, Meta, Amazon, and Apple](https://www.designgurus.io/blog/staff-engineer-levels?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): L6, E6, and ICT5 compared.
- Free article: [System design interview for L6 engineers](https://www.designgurus.io/blog/system-design-interview-l6-engineers?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): what interviewers expect at staff level.
- Free article: [The seven questions staff engineers ask](https://www.designgurus.io/blog/seven-questions-staff-engineers-ask?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): what to settle before drawing a single box.
- Free article: [System design trade-offs](https://www.designgurus.io/blog/complex-system-design-tradeoffs?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): how a senior engineer reasons through them.
- Free article: [Behavioral interview guide for large tech companies](https://www.designgurus.io/blog/faang-behavioral-interview-guide?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): question types and answer structure.

## Go deeper

This repository gives the outline. The course teaches each skill in full and ends every lesson with how to use it in an interview.

- [Grokking Staff Engineer Interview](https://www.designgurus.io/course/grokking-staff-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): lessons on judgment, scope, and influence, with a worked design, a staff behavioral question bank, and full mock loops.
- [Advanced System Design Interview, Volume II](https://www.designgurus.io/course/grokking-system-design-interview-ii?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): advanced case studies for the system design round.
- [Advanced System Design Fundamentals](https://www.designgurus.io/course/advanced-system-design-fundamentals?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): migrations, cost estimation, and designing under ambiguity.
- [Grokking Modern Behavioral Interview](https://www.designgurus.io/course/grokking-behavioral-interview?utm_source=github&utm_medium=repo&utm_campaign=staff-engineer-interview&utm_content=readme): the STAR method, a story bank, and company frameworks.

Related free guides: [Grokking System Design](https://github.com/design-gurus/grokking-system-design), [Engineering Manager Interview](https://github.com/design-gurus/engineering-manager-interview), and [Amazon Leadership Principles](https://github.com/design-gurus/amazon-leadership-principles).

For the system design round, see [Grokking System Design](https://github.com/design-gurus/grokking-system-design), the free companion guide with 30 patterns, 59 question walkthroughs, and 35 cheat sheets.

## More free guides

Every guide below is free, follows the same short-page format, and comes from DesignGurus.io.

- **Core guides:** [Grokking System Design](https://github.com/design-gurus/grokking-system-design), [Grokking Coding Interview](https://github.com/design-gurus/grokking-coding-interview), [Grokking AI System Design](https://github.com/design-gurus/grokking-ai-system-design), [Design Patterns](https://github.com/design-gurus/design-patterns), [Best System Design Resources](https://github.com/design-gurus/best-system-design-resources), [Best System Design Courses](https://github.com/design-gurus/best-system-design-courses)
- **By interview round:** [System Design Numbers](https://github.com/design-gurus/system-design-numbers), [API Design Interview](https://github.com/design-gurus/api-design-interview), [Frontend System Design Interview](https://github.com/design-gurus/frontend-system-design-interview), [Mobile System Design Interview](https://github.com/design-gurus/mobile-system-design-interview), [Microservices Interview Questions](https://github.com/design-gurus/microservices-interview-questions), [Concurrency Interview](https://github.com/design-gurus/concurrency-interview)
- **By role:** [DevOps and SRE Interview](https://github.com/design-gurus/devops-sre-interview), [Data Engineering Interview](https://github.com/design-gurus/data-engineering-interview), [Forward Deployed Engineer Interview](https://github.com/design-gurus/forward-deployed-engineer-interview), [Solutions Architect Interview](https://github.com/design-gurus/solutions-architect-interview)
- **Seniority and behavioral:** [Engineering Manager Interview](https://github.com/design-gurus/engineering-manager-interview), [Amazon Leadership Principles](https://github.com/design-gurus/amazon-leadership-principles), [Software Engineer Levels](https://github.com/design-gurus/software-engineer-levels)
- **By company:** [Google Interview Guide](https://github.com/design-gurus/google-interview-guide), [Meta Interview Guide](https://github.com/design-gurus/meta-interview-guide), [Amazon Interview Guide](https://github.com/design-gurus/amazon-interview-guide), [Microsoft Interview Guide](https://github.com/design-gurus/microsoft-interview-guide), [Apple Interview Guide](https://github.com/design-gurus/apple-interview-guide), [Netflix Interview Guide](https://github.com/design-gurus/netflix-interview-guide), [OpenAI Interview Guide](https://github.com/design-gurus/openai-interview-guide)

## Contributing

Corrections, new questions, and reports of how a staff loop was run are welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request.

## License

The content is licensed under [CC BY 4.0](LICENSE). See [NOTICE.md](NOTICE.md) for what the license covers and how to attribute.
