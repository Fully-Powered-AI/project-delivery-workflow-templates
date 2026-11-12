# Project intake and capacity review

When a new initiative is proposed, the portfolio owner sees it scored on the business's own criteria beside the projects already committed, the delivery days it would use month by month, and what it would crowd out or push later. The owner accepts, defers or rejects it.

*Workflow template · Project and delivery · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflow templates/project-intake-and-capacity-review/)*

## The outcome

A proposal stops being a matter of who argued best in the meeting. The portfolio owner gets a short review that places the new initiative in the same ranking as everything already committed, using the criteria the business has already agreed on, with the evidence behind every score quoted from the proposal itself.

Beside the ranking sits the cost in delivery days. For each role and each month, the page shows the load with and without the proposal, how much room is left under the ceiling the business set, and, where the proposal pushes a role over it, which committed projects use that role that month, lowest score first, with fixed work kept apart because it cannot move. It also tests later start months, so the owner can see whether waiting would make the proposal fit.

The portfolio owner reads it and decides: accept, defer or reject. The page lays out the facts for each choice and recommends none of them. The AI assistant changes no plan, tells no one and schedules nothing.

## Who starts the work, and when

The portfolio owner or the operations lead runs it when a proposal arrives and before anyone commits to it, usually at the monthly portfolio review or whenever a leader asks for a new project to be taken on. The portfolio owner reads the result the same week.

## What they supply

- The proposal as written, and the date it should start.
- The list of committed projects, with their dates, whether each is fixed, and their scores on the business's criteria.
- The delivery days each committed project uses, by role and month.
- The days each role has available each month, after leave and ongoing run work.
- The business's criteria, their weights, what each score from 1 to 5 means, and the ceiling for load.
- The delivery days the proposal would need, by role and month, and who estimated them.

## What comes out

A short review, up to two pages, in a fixed order: the proposal in brief, its score ranked among the committed projects with the evidence for each score, the monthly load by role, the over-ceiling months with the committed work that would have to give way, the start months tested, the gaps and questions, and the decision laid out for the portfolio owner. Any section with nothing to report says so. If the capacity or the project export does not match the expected headings, nothing is calculated until someone says which column is which.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Professional services](https://fullypowered.ai/industries/professional-services/), where the same few people serve client work and internal projects and each new idea takes days from both.
- [Marketing and advertising](https://fullypowered.ai/industries/marketing-and-advertising/), where design and build time is the scarce thing and every campaign or tool request competes for it.
- [Software technology](https://fullypowered.ai/industries/software-technology/), where developer days are the limit and the roadmap has more asks than days.
- [Engineering firms](https://fullypowered.ai/industries/engineering-firms/), where internal improvement projects draw on the same engineers as billable work.
- [Project and delivery](https://fullypowered.ai/functions/project-and-delivery/), which owns the committed list and the dates.
- [Operations and process improvement](https://fullypowered.ai/functions/operations-and-process-improvement/), where improvement ideas arrive faster than anyone can staff them.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where new initiatives land on a team that is already full.
- [Growth and scaling](https://fullypowered.ai/situations/growth-and-scaling/), where the number of good ideas passes the number of available people.

## What has to change for your company

Write your own criteria and weights, and say in a line what a 1, a 3 and a 5 mean on each, so two people would score the same proposal alike. Choose the load ceiling. Decide the roles you plan by and whether a month or a week is the period. Mark which committed work is fixed and who may say so. Settle who receives proposals, who may score them and who accepts, defers or rejects. Keep one source for the committed list and for available days; when the page and that source disagree, the source wins.

## What has been checked

Fully Powered AI wrote this workflow template, drawing on one published open-source method credited in its sources. It was editorially reviewed on 10 November 2026. It was tried once on its invented example in Claude on 10 November 2026, and the record of that run is published with it. The run produced every part of the review and reached no stop condition; the acceptance tests in the template were not run. After an earlier run, the example was made to say where its count came from, the scoring of a goal and the treatment of a 0-day row were settled in the instructions, and the run on this version is the one recorded. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on two or three past proposals whose outcome you already know, with hard cases written in advance: a proposal with no stated benefit, a role already over its ceiling before the proposal, fixed work that makes the gap unsolvable, a capacity export with a renamed column. The portfolio owner checks every score and every day count before anyone relies on it. [Project status report](https://fullypowered.ai/workflows/project-status-report/) then reports on a project once it is running, and [Headcount plan](https://fullypowered.ai/workflows/headcount-plan/) is the place to look when the answer to a capacity gap is more people.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 10 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 10 November 2026. The record is in [TRIAL.md](TRIAL.md).
- Not yet tested in a client environment.

## What is in this folder

- [TEMPLATE.md](TEMPLATE.md): the complete workflow template. Roles, inputs, the procedure, exceptions and stop conditions, the output format, a reviewer checklist, acceptance tests, the instructions for an AI assistant and what to customize.
- [EXAMPLE.md](EXAMPLE.md): a worked example with invented data.
- [TRIAL.md](TRIAL.md): what came out when the template was tried on its example.
- [SKILL.md](SKILL.md): the technical file, for AI products that load packaged instructions from a folder.
- [SOURCES.md](SOURCES.md): what the workflow template drew on, with licences.
- [LICENSE](LICENSE): MIT. Use it, change it, make it yours.

## Start using it

1. Read [EXAMPLE.md](EXAMPLE.md) to see what a good result looks like.
2. Open [TEMPLATE.md](TEMPLATE.md) and set every item under "What to customize" to your own rules, roles and limits.
3. Give your AI assistant the instruction block and the output format from the template, with your own limits in place of the ones the instructions leave open in square brackets. Paste them in as custom instructions in ChatGPT, Claude, Copilot or Gemini, or copy this whole folder into a product that loads `SKILL.md` packages. This folder stands alone; you do not need the rest of the repository.
4. Run it on past work first, using the reviewer checklist and acceptance tests in the template, before anyone relies on it.

## Related workflow templates

- [Project status report](../project-status-report/)
- [Headcount plan](https://fullypowered.ai/workflow templates/headcount-plan/)
- [Workflow fit check: is this piece of work ready for AI?](https://fullypowered.ai/workflow templates/workflow-fit-check/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
