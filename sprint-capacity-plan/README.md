# Sprint plan against capacity

Before each planning meeting, the delivery lead or scrum master brings a draft plan for the next sprint: the days each person really has, a forecast from the team's own recent delivery, the carryover, the ranked backlog cut at that figure, and what each item waits on. The team decides the commitment.

*Workflow template · Project and delivery · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/sprint-capacity-plan/)*

## The outcome

The planning meeting starts from a page instead of a blank board. Everyone sees how many working days the sprint holds once weekends, holidays and each person's time away are taken out, what the team actually finished in its last few sprints, and the figure that gives for this one, with a low and a high end so the risk is visible.

Work left over from the sprint that is ending goes in first, at the size it still needs. Then the backlog follows in the product owner's approved order until the planning figure is reached, and the line is drawn there. Nothing is skipped to squeeze in a smaller item; that choice is put to the team as a question. Items that are not ready, have no estimate, are held back or wait on unfinished work on the same board are set aside, each with its reason.

Every assumption behind the numbers is written down, and every open point arrives as a question with its facts. The team confirms the estimates and the dependencies and decides what it commits to, with the product owner. The AI assistant changes nothing on the board, assigns no one and commits nothing.

## Who starts the work, and when

The delivery lead, scrum master or team lead runs it once the ending sprint's work has stopped and the board has been exported, a day or two before the planning meeting. It runs again if the order, an estimate or someone's availability changes before the meeting. Any team that plans in fixed sprints of one to four weeks can use it, whether it builds software, campaigns, designs or client deliverables.

## What they supply

- **The settings:** the sprint's dates, the closed days inside it, the estimate unit (points, hours or days), which statuses mean done and ready, and whether to plan to the forecast, its low end or a figure the team sets.
- **The board export,** as a CSV file or pasted table with set column headings: key, title, status, estimate, remaining, rank, assignee, sprint and what each item depends on. If a heading does not match, nothing is calculated until someone says which column is which.
- **Team availability:** each person, their role, the share of their time that goes to this team and the dates they are out. Dates only; never a reason.
- **Recent delivery,** as an export or a short table: for the last few sprints, the person-days available, what was committed and what was completed.
- **The product owner's notes:** the sprint goal, what must be included and what is held back.

## What comes out

One draft in a fixed order: the capacity, with the working days, each person's person-days and the forecast with its range; the carryover; the draft plan in order with a running total and the planning line; the items below the line and those set aside, each with its reason; what each item waits on; the product owner's notes checked against the draft; the load by person; the assumptions; and the questions for the team. Any section with nothing in it says so.

When estimates are in hours or days, the load by person shows whether anyone is assigned more than their share. When they are in points, it makes no such comparison, because points measure the team's work, not one person's. The draft never compares one person's output with another's.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Project and delivery](https://fullypowered.ai/functions/project-and-delivery/), which runs the planning meeting and keeps the iteration rhythm.
- [Software engineering](https://fullypowered.ai/functions/software-engineering/), where the backlog, the carryover and the dependencies between items decide what a sprint can hold.
- [Software technology](https://fullypowered.ai/industries/software-technology/), where product teams plan in sprints and a holiday week leaves fewer days than the board assumes.
- [Marketing and advertising](https://fullypowered.ai/industries/marketing-and-advertising/), where agency and in-house teams run campaigns and content in sprints and share designers across teams.
- [E-commerce and retail](https://fullypowered.ai/industries/ecommerce-and-retail/), where the store's own team plans site and catalogue work in sprints around trading peaks.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where delivery teams work client implementations in sprints and lose people to other engagements.
- [Growth and scaling](https://fullypowered.ai/situations/growth-and-scaling/), when new teams form and need a planning habit that holds up.
- [Startups and new ventures](https://fullypowered.ai/situations/startups-and-new-ventures/), where a small team with part-time members has to plan honestly from the start.

## What has to change for your company

Map your board's column names to the template's once and keep the map with the settings. Name your done and ready statuses. Decide how many past sprints make the forecast, and whether you plan to the forecast, its low end or a figure the team chooses. Say how part-time members and people shared with other teams are counted. Decide whether carried work goes ahead of new work, which is the default, or takes its place by rank. Agree who may change the order before planning and who updates the board afterwards. It works in ChatGPT, Claude, Copilot or Gemini from the files you supply, with no connection to your board.

## What has been checked

Fully Powered AI wrote this workflow template from its own published map of the work. It was editorially reviewed on 11 November 2026. It was tried once on its invented example in Claude on 11 November 2026, and the record of that run is published with it. The run reached no stop condition; the acceptance tests were not run. It has not yet been tested in a client environment, and has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on two or three past sprints your team remembers well, plus hard cases written in advance, each with its expected behaviour: a sprint with a holiday inside it, a renamed column in the board export, carried work with no remaining size, an item ranked high that waits on unfinished work, a team with only one past sprint. The delivery lead checks every figure against the board and the calendar before the team relies on the draft. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 11 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 11 November 2026. The record is in [TRIAL.md](TRIAL.md).
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

- [Project intake and capacity review](../project-intake-and-capacity-review/)
- [Roadmap tradeoff review](https://fullypowered.ai/workflows/roadmap-tradeoff-review/)
- [Acceptance criteria sheet](https://fullypowered.ai/workflows/acceptance-criteria-sheet/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
