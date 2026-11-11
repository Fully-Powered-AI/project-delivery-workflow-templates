# Project scope baseline

A project manager turns an approved brief into a draft scope baseline: the deliverables, what is excluded, the acceptance criteria for each deliverable, the constraints and the open questions for the sponsor. Nothing implied counts as scope until the sponsor says so.

*Capability template · Project and delivery · version 0.1.0 · [Capabilities Directory](https://fullypowered.ai/capabilities/project-scope-baseline/)*

## The outcome

The project manager and the sponsor sit down with one page that is clear enough to disagree with. Every deliverable the brief names is listed once, with the tests a person can run to say it is accepted and the role that accepts it. What is out of scope is written down beside what is in. The limits on the project, such as budget, dates, people and platform, are listed with where each came from.

The part that earns its keep is the questions. Wherever a conversation, a note or the sponsor's own expectation reaches past the brief, the draft does not quietly add it and does not quietly drop it. It becomes a question with the facts beside it, and it stays a question until the sponsor answers. The same holds for a vague test such as "easy to use": the draft quotes the words and asks what would be accepted instead.

The project manager and the sponsor agree scope and acceptance before the baseline is set. The draft prints its sign-off lines empty, and the AI assistant never fills them in.

## Who starts the work, and when

The project manager runs it once the brief is approved and before planning the delivery in detail. It suits any project that has a brief, a sponsor and more than one deliverable: a system change, an office move, a new service, a client implementation run by your own team. The project manager reads the draft first, settles what they can, and takes the rest to the sponsor.

It writes a first baseline only. Changes to scope after the baseline is agreed belong to the project's change control. Until then it can be run again if the brief is reissued; the sponsor's answers to the questions are recorded by the project manager and agreed in the baseline, not fed back in.

## What they supply

- **The approved brief,** pasted or attached, with its approval date.
- **Discovery notes,** if any: what was learned in conversations after the brief was written.
- **Constraints,** if any: budget, dates, people who are away, platform limits, rules the project must follow.
- **The sponsor's expectations,** if any, in the sponsor's own words.
- **A working deliverable list,** if the project already has one, as a spreadsheet export with the columns ID, Deliverable, Source and Status.
- **Settings:** the project name, the sponsor's role, the project manager's role and the date.

## What comes out

A draft in a fixed order: a status line that says "draft, not baselined" and counts the questions that block baselining; the deliverables, each with its acceptance criteria and who accepts it; the exclusions; the constraints; the open questions for the sponsor; anything set aside because it is not scope; and an empty sign-off block for the project manager and the sponsor. Empty sections say so in a few words, so the reader knows nothing was left out.

It is an internal working document. It is not a client statement of work and it is not a contract, and it does not become one when it is signed off.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Project and delivery](https://fullypowered.ai/functions/project-and-delivery/), where the first piece of work after approval is agreeing what the project will and will not deliver.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where internal projects and client implementations both start from a short brief.
- [Software and technology](https://fullypowered.ai/industries/software-technology/), where "done" for each deliverable is argued about most.
- [Engineering firms](https://fullypowered.ai/industries/engineering-firms/), where an internal system or process change has to be scoped between project deadlines.
- [Construction](https://fullypowered.ai/industries/construction/), for the office-side and yard-side projects a contractor runs for itself.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where the sponsor has little time and needs one page to react to.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when the company begins running several projects at once and briefs get looser.

It sits before [Pilot acceptance-test preparation](https://fullypowered.ai/capabilities/pilot-acceptance-test-preparation/), which sets up the tests for an AI pilot, and before [Project status report](https://fullypowered.ai/capabilities/project-status-report/), which reports against the plan once it exists. [Decision log](https://fullypowered.ai/capabilities/decision-log/) keeps the sponsor's answers to the open questions.

## What has to change for your company

Decide who counts as the sponsor and who may accept a deliverable; the draft asks, and your answer becomes the default. List the words your company treats as too vague to test, and add them to the draft's list. Choose the form your constraints take, for example whether a budget is one figure or split by phase. Decide which questions you will let the project manager settle alone and which always go to the sponsor. It runs in ChatGPT, Claude, Copilot or Gemini from the documents and notes you supply; it needs no connection to your project software.

## What has been checked

Fully Powered AI wrote this capability template from its own published map of the work, with no third-party text. It was editorially reviewed on 10 November 2026. It was tried once on its invented example on 10 November 2026 in Claude, and the record is published with it. The run showed the same four deliverables, the same two exclusions from the brief and the same $30,000 working; it differed on the blocking count (9 against the example's 8) and on how the shared-drive and invoice-payment remarks were classified. The edits made after that run, to the instructions on those points, to the wording of a few rules and to the example, have not been run again. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on the brief of a project you finished and remember well, then checking the draft against what the team and the sponsor argued about later: the deliverable nobody listed, the exclusion nobody wrote down, the acceptance test that was never agreed. The project manager checks every line against the sources before the draft goes to the sponsor. [Pilot acceptance-test preparation](https://fullypowered.ai/capabilities/pilot-acceptance-test-preparation/) sets up cases like these.

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
- [Decision log](https://fullypowered.ai/capabilities/decision-log/)
- [Pilot acceptance-test preparation](https://fullypowered.ai/capabilities/pilot-acceptance-test-preparation/)

## Make it yours

This is the starting version. Fully Powered AI adapts capabilities to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
