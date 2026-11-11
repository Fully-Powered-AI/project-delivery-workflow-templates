# Project handover readiness check: tried on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Sonnet 5.5 (claude-sonnet-5-5), by Anthropic.
- **Date:** 2026-11-10
- **Template version:** 0.1.0

This trial used only the invented example in `public/example.md`: the handover settings, the requirements list and the five registers (evidence, access, training, support owners, open items). No client data was used. The model that ran it did not write the template. It read the template and the example's inputs first, produced the checklist by following the instruction block and the output format, and only then compared its checklist with the example's published output and the reviewer checklist.

## What came out

```
HANDOVER READINESS CHECK: Inspection scheduling system

For: Scheduling manager, Scheduling team. Prepared by: Project manager, operations projects.
Check date: Thursday 12 November 2026. Planned handover: Monday 16 November 2026. Project team support ends: Friday 11 December 2026.
Supplied: requirements (10, 7 must-have); evidence register (8 rows); access list (4 rows); training record (4 rows); support owners (4 rows); open items (4 rows).

Position by the rules: 1 of 7 must-have requirements met. Conditions open: 6. For the Scheduling manager to judge: 1. Not must-have and still open: 1. This is a count, not a decision.

Requirements

Acceptance
R01 User acceptance test passed and signed off (must-have). Expected: sign-off by Scheduling manager. Status: Partly met. Evidence: E01 test summary, 46 of 48 scripts passed, Friday 6 November; E02 note, sign-off meeting booked for Friday 13 November, Tuesday 10 November (a note, not counted). Finding: no sign-off by the Scheduling manager; E01 is a test record and shows 2 failed scripts, logged as OI-02 and OI-03.
R02 Load test at 400 bookings a day or more (not must-have). Expected: test record. Status: Met. Evidence: E03 load test, 450 simulated bookings in one day with no failed booking, Wednesday 4 November. Finding: nothing missing.

Instructions
R03 Daily operating guide for schedulers (must-have). Expected: document. Status: Met. Evidence: E04 daily operating guide version 1.2, Monday 9 November. Finding: nothing missing.
R04 A scheduler has run the morning schedule build from the guide without help (must-have). Expected: demonstration. Status: Not evidenced. Evidence: E05 operating guide section 2, a document, Monday 9 November. Finding: document only: nobody in the receiving team is recorded doing it.
R09 Supplier contacts and escalation route written down (not must-have). Expected: document. Status: Not evidenced. Evidence: E06 Supplier A contacts and escalation route, a document, undated. Finding: undated.

Access
R05 Scheduling team holds the access it needs to run and administer the system (must-have). Expected: access granted. Status: Partly met. Evidence: access list, 4 rows linked. Finding: 2 of 4 rows granted. Not granted: Scheduling system, Administrator (backup), Senior scheduler, requested Monday 9 November; Supplier A support portal, Named contact, Scheduling manager, not requested, no date.

Training
R06 Every scheduler trained and has run a live day unaided (must-have). Expected: ran unaided. Status: Not met. Evidence: training record, 4 rows linked. Finding: Scheduler D has no trained date (not trained). Scheduler C: trained Thursday 29 October; ran unaided dated Friday 13 November, dated after the check date. Schedulers A and B: trained and ran unaided.

Support
R07 Every support topic has an owner after handover who has agreed to it (must-have). Expected: owner accepted. Status: Not met. Evidence: support owners, 4 rows linked. Finding: Changes to booking rules and templates: Senior scheduler named, not accepted. Also, Supplier A account and renewals: cover from Monday 4 January 2027, after the cover limit of Saturday 12 December 2026.
R10 Response time for system faults agreed with IT (not must-have). Expected: service levels confirmed by IT lead. Status: Owner to judge. Evidence: E07 note from the IT lead, faults reported before 2 pm are answered the same working day, Tuesday 10 November. Finding: the expected evidence is outside the fixed list; for the Scheduling manager to judge.

Open items
R08 Every open item has an owner after handover and no high-severity item is left without a workaround (must-have). Expected: owners and workarounds. Status: Not met. Evidence: open items, 4 rows linked. Finding: OI-03 is high severity with no workaround. OI-04 has no owner after handover.

Conditions still to meet (proposed)
R01: the Scheduling manager's sign-off of the user acceptance test is recorded; the test summary shows 2 of 48 scripts failed. Owner and date: for the Scheduling manager to set.
R04: a member of the scheduling team is recorded running the morning schedule build from the guide without help. Owner and date: for the Scheduling manager to set.
R05: the Senior scheduler's Administrator (backup) access is granted, and the Scheduling manager's named contact on the Supplier A support portal is requested and granted. Owner and date: for the Scheduling manager to set.
R06: Scheduler D is trained; Scheduler D and Scheduler C have each run a live day unaided on or before the check. Owner and date: for the Scheduling manager to set.
R07: the Senior scheduler has agreed to own changes to booking rules and templates, and Supplier A account and renewals has an agreed owner covering Saturday 12 December 2026 to Sunday 3 January 2027. Owner and date: for the Scheduling manager to set.
R08: OI-03 has a workaround, and OI-04 has an owner after handover. Owner and date: for the Scheduling manager to set.

Also open (not must-have)
R09: Not evidenced. E06 is undated.

For the Scheduling manager to judge
R10 Response time for system faults agreed with IT. Expected: service levels confirmed by IT lead. Supplied: E07, a note from the IT lead saying faults reported before 2 pm are answered the same working day, Tuesday 10 November. Question: does this meet the requirement?

Support after handover
Day-to-day scheduling questions: Scheduling manager, accepted, cover from Monday 16 November 2026.
System faults and outages: IT lead, accepted, cover from Monday 16 November 2026.
Changes to booking rules and templates: Senior scheduler, named, not accepted, cover from Monday 16 November 2026.
Supplier A account and renewals: Operations director, accepted, cover from Monday 4 January 2027. Gap: Saturday 12 December 2026 to Sunday 3 January 2027, 23 days.

Open items carried into operation
OI-02 (high) Repeat bookings that fall on a public holiday are not moved. Workaround: schedulers check holiday weeks by hand (guide section 5). Owner after handover: Scheduling manager. Due: Friday 27 November 2026.
OI-03 (high) Cancellation emails to clients show the old office address. Workaround: none. Owner after handover: Supplier A. Due: Friday 20 November 2026.
OI-01 (medium) Calendar updates reach inspectors' phones up to 15 minutes late. Workaround: inspectors refresh the app before leaving. Owner after handover: IT lead. Due: Friday 4 December 2026.
OI-04 (low) Monthly utilisation report not yet built. Workaround: none. Owner after handover: not assigned. Due: not stated.

Supplied but not linked
E08: data move check, 1212 of 1212 open bookings moved from the old diary, test record, Monday 2 November. No requirement named.

Decision of the Scheduling manager (left blank for them)
[ ] Accept the handover   [ ] Accept with the conditions above   [ ] Not accepted yet
Name, role and date: ____________

Prepared for the Scheduling manager's decision. Nothing has been granted, removed, signed, sent or changed.
```

## What was observed

- **Every required part was produced,** in the fixed order, with the empty-section wording not needed because every section had content. Nothing in the inputs made the instructions stop: the settings were complete, headings matched, no id repeated, every area was one of the six and no secret was present.
- **Statuses and counts matched the published example.** Both give 1 of 7 must-haves met, 6 conditions, 1 requirement for the receiving owner to judge and 1 not-must-have still open. The 23-day support gap, the open-item order and the one unlinked row (E08) also match.
- **Differences from the published example, all small.** These compare with the example as it stood at the time of the run; it has since been hand-edited, as the last section discloses, so today's `public/example.md` may differ in these places:
  - The R05 finding here says the "not requested" row has "no date"; the example leaves the blank date out.
  - The R06 condition here says Scheduler C and D have each run a live day unaided; the example words it as Schedulers C and D each running one. My wording adds "on or before the check", which is not in the rules and is clumsy; the example's is cleaner.
  - The R05 condition here says "requested and granted" for the portal contact; the example says only "granted".
  - The R04 condition here says "recorded running" a build; the example says "recorded as a demonstration".
  - The R07 finding here opens its second sentence with "Also", the example does not.
  - The condition for R01 here leaves out the references to OI-02 and OI-03; the example keeps them.
- **Facts not in the inputs.** None in either output. Weekdays are worked out from the check date, and every other fact traces to an input row. The condition wordings add no new fact.
- **Where the instructions were ambiguous and a guess was needed:**
  1. When a support requirement is Not met for one reason (an unaccepted owner) and a second reason also applies (cover starting after the cover limit), the rules do not say whether to mention the second in the finding. It was mentioned, as the example does. The gap is shown under "Support after handover" and in the condition either way.
  2. The format says an unmet access row is given "with its status and date" but not what to write when the date is blank. "No date" was used.
  3. The position line's "Not must-have and still open" does not say whether an "Owner to judge" requirement counts. It was left out, because step 9 keeps those two groups apart; the example does the same, but the line does not say it.
  4. A linked row that does not count (here E02, a note against a sign-off) is to be "listed under Evidence", but the format does not say how to mark it as not counted. A bracketed note was added.
  5. An access row can stand for a group of people ("4 schedulers"); the rules do not say how a group row is counted. It was counted as one row.
  6. The conditions are to be "built only from the finding", but the exact shape of a condition is left to the writer, so wording differed from the example in the small ways listed above.
- **Stops.** The instructions asked for no stop on these inputs. The acceptance tests that cover stops (no list, renamed heading, a password, being asked to decide) were not run in this trial.
- **Shortcomings.** This was one run, by one model, on one invented example. It shows the instructions produce a checklist whose statuses and counts agree with the published one. It does not show the template works with a real project's files, with messier headings, or in another product. It is not a test for a client.

## Edits made after this run, and not run again

The output and observations above are as recorded. After an independent review, on 10 November 2026, the template was edited in small ways that have not been run again:

- The rule for dates after the check date now names the columns it applies to: evidence dated, the date of a granted access row, trained_on and ran_unaided_on.
- The access rule now says a row that stands for a group counts as one row, and that a row with no date is written "no date" (ambiguities 2 and 5).
- A linked row that does not count is now marked "(not counted: [why, in a few words])" in the output format (ambiguity 4). The run used a different bracketed note, "(a note, not counted)".
- The owner-accepted rule now says to name every reason that applies (ambiguity 1).
- The position line rule now says an Owner to judge requirement is counted only under the owner's judgement, not under "Not must-have and still open" (ambiguity 3), and the pasted instructions now carry the "undated" and "not trained" wordings and the naming of each person who falls short on ran unaided.
- The published example was brought into line with those edits: it now carries the "(not counted: [why])" mark on E02, E05 and E06 and "no date" on the R05 row not requested. It was not re-run; only those marks were added by hand.
- The pasted instructions now also carry two finding details the procedure already had: who signed, for a sign-off by the wrong role, and the count of granted access rows with each row not granted.
- After a second review, a requirement with no linked row in the register its rule names is now stated to be Not evidenced for the access granted, ran unaided and owner accepted rules (the template and the pasted instructions), and the pasted instructions now carry the sentence that whether a document's content is good enough is for the receiving owner. The example has no such requirement, so its output is unchanged. Not run again.
