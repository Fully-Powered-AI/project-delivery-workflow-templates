# Schedule recovery options

When a committed milestone slips, the project manager brings the sponsor two to four ways back: what each changes, the dates it gives every later milestone and dependency, and the assumptions it rests on. The sponsor chooses; delivery leads confirm the dates.

*Capability template · Project and delivery · version 0.1.0 · [Capabilities Directory](https://fullypowered.ai/capabilities/schedule-recovery-options/)*

## The outcome

The sponsor does not get a slipped date and a request to "find the time". They get the slip stated plainly, what happens to every later date if nothing is done, and a short set of real choices set side by side: cut or defer scope, change the order of work, add people, or move the date. Each choice shows the new dates of the milestones behind it, the outside commitments it touches and the day by which someone must ask a supplier or another team to change theirs.

Each option also says what it assumes. Cutting a module assumes the people who rely on it have a workable fallback. Adding a tester assumes the work can be split and that a newcomer needs a few days to become useful. Where options act on the same stretch of work, the page recomputes them together instead of adding their savings, so the sponsor never sees a recovery that does not exist.

The project manager reads the draft, corrects it with the delivery leads and decides what goes to the sponsor. The AI assistant changes no plan, promises nothing to anyone and recommends no option unless the company's settings allow it and the sponsor asks.

## Who starts the work, and when

The project manager starts it as soon as a milestone the project has committed to is forecast to miss its date, before the sponsor is asked to react. It suits any project with a dated plan, dependencies and a sponsor above it: a system replacement, a fit-out, a new service, an office move. The delivery leads confirm the dates the same week, and the sponsor chooses at the next decision point.

## What they supply

- **The schedule,** exported as a spreadsheet: each task and milestone with its dates, baseline finish, duration, remaining work, predecessors and who the date was committed to.
- **The slip:** which milestone, the date committed, the new forecast and the cause as the person reporting it gave it.
- **The scope list,** with a priority for each item and what happens if it is deferred.
- **Who could help,** with the days each person is available and the tasks they could join.
- **Outside commitments:** each dependency on a supplier or another team, the date promised, whether they accepted it and how much notice a change needs.
- **Fixed dates and the working calendar,** with holidays and any freeze periods.
- **The settings:** the sponsor and delivery leads, today's date, the date of the schedule export, who has already been told the current date, and who confirms a deferral that touches their area.

## What comes out

One page for the sponsor, in a fixed order: the slip, what happens if nothing changes, then each option with its change, the working days it recovers, the dates it gives each later milestone, the dependencies it touches, its assumptions, what it costs and who must confirm it. Combinations are computed, never added up. What is not known is listed as questions. Sections with nothing in them say "None".

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Project and delivery](https://fullypowered.ai/functions/project-and-delivery/), where the plan is the promise and a slip has to be answered with choices, not reassurance.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where client work and internal projects compete for the same people.
- [Construction](https://fullypowered.ai/industries/construction/), where a late task moves the trades and deliveries behind it.
- [Engineering firms](https://fullypowered.ai/industries/engineering-firms/), where a missed design milestone ripples through reviews and releases.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when more projects run at once than anyone can hold in their head.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where fixed dates such as renewals, closes and seasons limit the choices.

It stays distinct from [Project status report](https://fullypowered.ai/capabilities/project-status-report/), which reports where the project stands, and from [Premortem before a decision](https://fullypowered.ai/capabilities/premortem-before-a-decision/), which looks for how a plan could fail before it is approved. This one starts after a date has already been missed.

## What has to change for your company

Decide who counts as the sponsor and who counts as a delivery lead for each option. Set your working calendar, your freeze periods and the notice each supplier or team needs for a change. Agree how many working days a newcomer needs before they help, and which kinds of task your people accept can be split. Name the priority labels your scope list uses and what fallback each deferred item must have before it can be offered. Settle whether the assistant may recommend an option when the sponsor asks; the default is that it declines.

## What has been checked

Fully Powered AI wrote this capability template. It was editorially reviewed on 10 November 2026. The dates in its worked example were recomputed from the example's inputs. It was tried once on its invented example in Claude on 10 November 2026; the record is published with it. That run was made by the same session that revised the example, so it was not independent, and it did not exercise the stop conditions, a range forecast, a missing export date or a latest date to ask that had already passed. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on a past slip your project manager already understands, with cases written in advance: an option that touches the same work as another, a supplier date nobody accepted, a freeze period that moves the answer. The delivery leads check every date before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/capabilities/pilot-acceptance-test-preparation/) sets those cases up, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 10 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 10 November 2026. The record is in [TRIAL.md](TRIAL.md).
- Not yet tested in a client environment.

## What is in this folder

- [TEMPLATE.md](TEMPLATE.md): the complete capability template. Roles, inputs, the procedure, exceptions and stop conditions, the output format, a reviewer checklist, acceptance tests, the instructions for an AI assistant and what to customize.
- [EXAMPLE.md](EXAMPLE.md): a worked example with invented data.
- [TRIAL.md](TRIAL.md): what came out when the template was tried on its example.
- [SKILL.md](SKILL.md): the technical file, for AI products that load packaged instructions from a folder.
- [SOURCES.md](SOURCES.md): what the capability drew on, with licences.
- [LICENSE](LICENSE): MIT. Use it, change it, make it yours.

## Start using it

1. Read [EXAMPLE.md](EXAMPLE.md) to see what a good result looks like.
2. Open [TEMPLATE.md](TEMPLATE.md) and set every item under "What to customize" to your own rules, roles and limits.
3. Give your AI assistant the instruction block and the output format from the template, with your own limits in place of the ones the instructions leave open in square brackets. Paste them in as custom instructions in ChatGPT, Claude, Copilot or Gemini, or copy this whole folder into a product that loads `SKILL.md` packages. This folder stands alone; you do not need the rest of the repository.
4. Run it on past work first, using the reviewer checklist and acceptance tests in the template, before anyone relies on it.

## Related capabilities

- [Project status report](https://fullypowered.ai/capabilities/project-status-report/)
- [Premortem before a decision](https://fullypowered.ai/capabilities/premortem-before-a-decision/)
- [Decision log](https://fullypowered.ai/capabilities/decision-log/)

## Make it yours

This is the starting version. Fully Powered AI adapts capabilities to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
