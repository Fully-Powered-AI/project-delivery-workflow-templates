# Project portfolio status roll-up

The head of delivery takes one page to leadership each fortnight or month, built from the reports project leads already write: every project red, amber or green as its own lead stated it, what moved, the decisions leadership is asked for, and where two reports contradict each other or a status has no reason.

*Workflow template · Project and delivery · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/portfolio-status-roll-up/)*

## The outcome

Leadership sees every project on one page, in the same shape every period, without anyone rewriting the leads' reports. Each project carries the colour its own lead gave it, the reason the lead gave, what finished since last time and the lead's forecast beside the planned end. A count at the top shows how many projects are red, amber and green, and which changed since the last roll-up.

The decisions come next, gathered from every report into one list ordered by the date each is needed. A question asked last period and still unanswered is carried forward with its number and marked when its date has passed, so nothing asked of leadership quietly disappears.

Then the part that is hardest to do by hand: where the reports do not fit together. When one project expects a handover from another on a date the other project's own report does not give, both statements are quoted side by side. A project that reports no colour, turns green without saying why, or sends nothing at all is listed by name, with the lead to ask.

The roll-up changes no status and adds no judgment of its own. It gives the portfolio no overall colour, ranks nothing and never says which of two reports is right. The head of delivery chases the gaps, confirms the page and decides what goes to leadership. The AI assistant sends nothing.

## Who starts the work, and when

The head of delivery or the head of operations, or a coordinator on their behalf, runs it once per reporting period, fortnightly or monthly, after the project leads' reports are in and before the leadership meeting. It suits a company of up to a few hundred people running several projects at once, each with its own lead: a new system, a new line, a move, a new service. It runs again if a late report arrives or a lead corrects a report after being asked about a gap.

## What they supply

- **The project register,** exported as a spreadsheet: each project with its ID, name, lead and planned end, and optionally its sponsor and the projects it depends on. If the column headings do not match the ones the workflow template expects, it stops and asks which column is which.
- **The project leads' status reports** for the period, as they wrote them. No fixed layout is needed.
- **The last roll-up,** so last period's colours and unanswered decisions carry over.
- **Leadership's decision notes** since the last roll-up.
- **The settings:** the period, the report date, the meeting date, who reads the page, the word limit, and, if your company uses words such as "on track" instead of colours, the agreed meaning of each.

## What comes out

One page for leadership in a fixed order: at a glance, the decisions asked of leadership, every project red first, then where the reports disagree or leave a gap. Empty sections say so in a word, such as "None found", so the reader knows nothing was left out.

Beneath it, a short part for the head of delivery only, removed before sending: who to chase before the meeting and about what, anything left out of the page and why, and a line to confirm every status was checked against its report.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Project and delivery](https://fullypowered.ai/functions/project-and-delivery/), which answers to leadership for every project at once, not one at a time.
- [Operations and process improvement](https://fullypowered.ai/functions/operations-and-process-improvement/), where the head of operations often holds the project list in a company without a delivery office.
- [Leadership](https://fullypowered.ai/functions/leadership/), which reads the page and owns the decisions on it.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where internal projects run beside client work and leadership wants them in one view.
- [Engineering firms](https://fullypowered.ai/industries/engineering-firms/), where a new system, a new office and a new service line can all be in flight in the same quarter.
- [Manufacturing](https://fullypowered.ai/industries/manufacturing/), where a new line, a warehouse move and a system change depend on each other's dates.
- [Software technology](https://fullypowered.ai/industries/software-technology/), where several product and internal projects report to one leadership team.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where projects run alongside a full working week and leadership has minutes for them, not hours.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when the company starts running more projects than one person can hold in their head.

## What has to change for your company

Decide who reads the page and how long before the meeting it goes out. Agree once whether your leads report in colours; if they write "on track" or "at risk", write down what each word means as a colour, or the roll-up will show the words and ask. Keep one project register as the list of who should report, with the projects each depends on, because that is where most contradictions are found. Decide whether the leads see the chase list before the meeting and how long they have to answer. Set the word limit to suit the number of projects. It runs in ChatGPT, Claude, Copilot or Gemini from files and notes you supply; it needs no connection to your project software.

## What has been checked

Fully Powered AI wrote this workflow template as an original method, with no third-party source. It was editorially reviewed on 12 November 2026. It was tried once on its invented example, in Claude on 12 November 2026; the run was not fully blind, and its record is published with it. The findings of that run were then acted on in the template's steps and instructions, and those edits have not been run again. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on two or three past periods your head of delivery remembers, with hard cases written in advance: a project that sends no report, a lead who writes "on track" instead of a colour, two reports that give different dates for the same handover, a decision from last time that nobody mentions. The head of delivery checks every status against the reports as written before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) sets up those cases, [Project status report](https://fullypowered.ai/workflows/project-status-report/) prepares each project's own report, and [Decision log](https://fullypowered.ai/workflows/decision-log/) keeps leadership's answers once they are given.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 12 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 12 November 2026. The record is in [TRIAL.md](TRIAL.md).
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
- [Project intake and capacity review](../project-intake-and-capacity-review/)
- [Decision log](https://fullypowered.ai/workflows/decision-log/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
