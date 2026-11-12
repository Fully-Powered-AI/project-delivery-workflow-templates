# Project handover readiness check

When a finished deliverable is ready for the team that will run it, the project manager brings one checklist against that team's own requirements: acceptance evidence, instructions, access, training, support owners and open items. The receiving owner accepts or names the conditions still to meet.

*Workflow template · Project and delivery · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/project-handover-readiness-check/)*

## The outcome

The handover meeting starts from facts instead of goodwill. Every requirement the receiving team wrote down sits on one page with a plain status beside it: met, partly met, not met, not evidenced, or for the receiving owner to judge. Every gap is spelled out: which access is still only requested, who has been trained but has not yet done the work alone, which support topic has a name against it but no agreement, which serious defect has no workaround yet.

The rules are strict where handovers usually go soft. A guide on file does not count as the team being able to do the work; someone from the receiving team has to have done it. A name in a plan does not count as an owner until that person has agreed. Anything planned for next week is planned, not done. When support cover would lapse between the project team leaving and the new owner starting, the checklist names the dates and counts the days.

Each unmet must-have arrives already written as a condition. The receiving owner decides: accept, accept with those conditions, or not yet. The AI assistant grants no access, signs nothing and decides nothing.

## Who starts the work, and when

The project manager starts it a few working days before the planned handover, once the deliverable has been tested and the handover pack is assembled, and runs it again on the day. The receiving owner, the manager whose team will run the result, reads the checklist and makes the call.

## What they supply

- **The handover details:** what is being handed over, to which team, the check date, the planned handover date and when the project team's own support ends.
- **The receiving team's requirements,** written by the receiving owner: each with its area, whether it is a must-have, and the evidence that would satisfy it.
- **The evidence register:** sign-offs, test records, guides and records of the receiving team doing the work, each dated.
- **The access list:** who in the receiving team holds which access, and whether it is granted, requested or not yet asked for. No passwords, ever.
- **The training record:** who was trained, and when each person first ran the work for real without help.
- **The support owners:** each topic, who owns it after handover, whether they have agreed, and from when.
- **The open items:** defects, known issues and unfinished work, with severity, workaround, owner and due date.

Each list has set column headings. If a heading does not match, the assistant stops and asks rather than guessing.

## What comes out

One checklist, in a fixed order. At the top, a count: how many must-haves are met and how many conditions are open. Then every requirement by area with its status, the evidence behind it and what is missing. Then the proposed conditions, each written as what must be true, with the owner and date left for the receiving owner. Then the support cover after handover with any gap in days, every open item carried into operation with the most serious first, and anything supplied that answers no requirement. It ends with a blank decision box for the receiving owner to complete.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Project and delivery](https://fullypowered.ai/functions/project-and-delivery/), which owns the moment a project's work becomes someone else's to run.
- [Operations and process improvement](https://fullypowered.ai/functions/operations-and-process-improvement/), often the team on the receiving end of a new system or a rebuilt process.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where internal projects hand new tools to the people who serve clients every day.
- [Software and technology](https://fullypowered.ai/industries/software-technology/), where a release passes from the people who built it to the people who support it.
- [Construction](https://fullypowered.ai/industries/construction/), where a finished site or system passes to the team that will operate and maintain it.
- [Engineering firms](https://fullypowered.ai/industries/engineering-firms/), where delivered systems and processes need an owner the day the project team moves on.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when new systems arrive faster than teams can absorb them.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where a handover too often means one email and a shared folder.

## What has to change for your company

The receiving owner writes the requirements list once for each kind of deliverable your teams take on, and adjusts it per project; the workflow template supplies no standard list. Agree the evidence each requirement may ask for and add any of your own. Set your severity scale and whether a medium item also needs a workaround. Decide whether the project team supports the result for a period after handover, and for how long. Decide who confirms that the project team's own access is removed, which this checklist does not cover as written. Name who signs the decision box and where the signed checklist is kept. It runs in ChatGPT, Claude, Copilot or Gemini from the lists you supply, with no connection to any system.

## What has been checked

Fully Powered AI wrote this workflow template from its own published map of the work. It was editorially reviewed on 10 November 2026. It was tried once on its invented example on 10 November 2026, and the record is published with it. Small edits made to the template after that run were not run again; the record lists them. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on two or three past handovers your receiving owners remember, plus hard cases written in advance, each with its expected result: a guide offered where a demonstration is required, a support owner who never agreed, a gap in support cover, a list with a renamed column, an access list with a password typed into it. The project manager and the receiving owner check every status and every date before anyone relies on the checklist. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) sets those cases up, and [SOP from how the work is done](https://fullypowered.ai/workflows/sop-from-how-the-work-is-done/) writes the operating guide the receiving team will need.

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

- [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/)
- [Write an SOP from how the work is done](https://fullypowered.ai/workflows/sop-from-how-the-work-is-done/)
- [Project status report](../project-status-report/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
