# Scope change impact review

When new work turns up in a project plan, the project manager gets one review: every deliverable compared with the agreed baseline, each addition marked approved or not, its estimated effect on effort, cost and the end date, and the decision the sponsor has to make. The sponsor accepts or declines each one.

*Workflow template · Project and delivery · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflow templates/scope-change-impact-review/)*

## The outcome

Extra work stops slipping into a project unseen. The project manager holds one page that shows what the plan contains today against what the sponsor agreed: which additions were approved, which arrived through a meeting, an email or a quiet edit to a deliverable, and which are already being worked on.

Each change that has not been decided comes with its price beside it: the days of effort, the cost at your day rate, and where the end date lands if that change alone is accepted. The sponsor sees a clear question for each one, "accept or decline?", with who asked for it and what it would take. A request agreed in a corridor is shown as a request, never as an approval, and two changes that each move the date are never added into one comfortable total.

The project manager checks the review and decides what the sponsor sees. The sponsor decides every change. The AI assistant edits no plan, estimates nothing itself and sends nothing.

## Who starts the work, and when

The project manager, or a project coordinator on their behalf, runs it whenever a deliverable appears in the working plan that the baseline did not have, when an agreed deliverable grows, and before each meeting where the sponsor rules on changes. It runs again after the sponsor's decisions are entered, to confirm the plan and the change log agree. It suits any project with an agreed scope and a sponsor: a client portal, an office move, a new system, a product launch.

## What they supply

- **The baseline:** the agreed deliverables with their due dates and effort, the end date, the budget, and the list of what was excluded from scope.
- **The working list** as it stands today, exported from the project tracker, with each deliverable's status.
- **The change log:** every decision on a change, who made it, when, and what it did to effort, cost and the end date.
- **The request notes:** the meeting notes, emails and messages where work was asked for.
- **The delivery lead's estimates** for each change not yet decided.
- **The settings:** who sponsors the project, who may approve a change, the day rate, working days and closed days.

The template names the column headings it expects and stops to ask when one does not match.

## What comes out

One review in a fixed order. At the top, the position: the baseline, the approved changes so far, and what is pending, in days, money and end date. Then the work already under way without approval, then the decisions for the sponsor, one per pending change, each with who asked, the effect and any match with something the baseline excluded. Then the full comparison with the baseline: unchanged, approved, not approved, declined but still in the plan, dates moved, and requests that never reached the plan. Empty sections say "none", so the reader knows nothing was skipped.

Beneath it, a short part for the project manager only, removed before sharing: the questions to settle first, such as who asked for an addition nobody can trace, or whether work started without approval carries on.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Project and delivery](https://fullypowered.ai/functions/project-and-delivery/), which holds the baseline and answers to the sponsor for every change to it.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where internal projects and client work compete for the same people's days.
- [Engineering firms](https://fullypowered.ai/industries/engineering-firms/), where a deliverable that quietly grows can take a team's slack before anyone notices.
- [Construction](https://fullypowered.ai/industries/construction/), for the office-side projects: a new estimating system, a new yard, a new reporting pack.
- [Marketing and advertising](https://fullypowered.ai/industries/marketing-and-advertising/), where requests arrive in every meeting and the plan absorbs them one at a time.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when more projects run at once and nobody has time to police each plan by hand.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where projects run beside a full working week and the sponsor needs the decision, not the history.

## What has to change for your company

Name who sponsors each project and which roles may approve a change; some companies let the project manager accept small changes under a set limit, and that limit should be written down. Set your day rate, or a rate per role if your estimates are split that way. Map your tracker's export and your change log to the headings the template expects, once. Agree how far ahead of the sponsor's meeting the delivery lead estimates each change, and whether work already done without approval goes to the sponsor or stays with the project manager. It runs in ChatGPT, Claude, Copilot or Gemini from files and notes you supply; it needs no connection to your project software.

## What has been checked

Fully Powered AI wrote this workflow template from its own published map of project and delivery work. It was editorially reviewed on 10 November 2026. It was tried once on its invented example on 10 November 2026 in Claude, and the run matched the example in every figure, date, order and count. It left a few points for judgement, which the published record lists: what the money figure in the position is, whether a moved date needs its own approval, and how to treat a change the requester made themselves. Small clarifications made afterward have not been run again. It has not yet been tested in a client environment, and not yet tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on two or three past changes your project manager remembers, plus hard cases written in advance: an addition agreed only in a meeting, a deliverable that grew from 40 items to 55, a declined change still in the plan, a change with no estimate, and two changes that each move the end date. The project manager checks every figure against the estimates and the change log before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) sets those cases up, and [Decision log](https://fullypowered.ai/workflows/decision-log/) keeps the sponsor's answers once they are given.

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
- [Decision log](https://fullypowered.ai/workflow templates/decision-log/)
- [Client-status update preparation](https://fullypowered.ai/workflow templates/client-status-update-preparation/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
