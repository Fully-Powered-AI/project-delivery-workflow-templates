# Schedule recovery options: tried twice on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5). The same session revised the template and the example, then made this run.
- **Date:** 2026-11-10
- **Template version:** 0.1.0, as revised on 10 November 2026 after an independent review (a read of the template and example by a reviewer who had not written them)

This is a record of runs of the capability template on its own invented example: Company A, an invented 45-person services firm, with an invented supplier, Vendor B. No client data was used. It is not a test in any company's environment.

This is the second run. The first run (earlier on 10 November 2026) used the template and example as first written; its output and observations are kept below as recorded. The run recorded immediately below was made on the revised template and the revised inputs in [public/example.md](example.md).

## Inputs used

Everything under "The inputs" in `public/example.md` as revised: the slip note (now stating that the monthly report the Reports module produces is Finance's), the schedule export, estimates and flexibility, scope list, list of who could help, outside commitments, fixed dates, and the settings, which now give today's date (Wed 16 Jun 2027), the export date (the same day) and who was told the current go-live date (Operations staff, Mon 19 Jul). Nothing else was supplied.

## What came out

```
SCHEDULE RECOVERY OPTIONS: Migration rehearsal complete (M1)

For: Managing director. Dates to be confirmed by: Test lead, Training lead, Operations lead (Finance lead for any deferral that affects Finance). Prepared Wed 16 Jun 2027 from the schedule export of Wed 16 Jun 2027.

The slip: M1 was committed for Fri 18 Jun and is now forecast for Fri 2 Jul, 10 working days late. Cause as reported: the migration rehearsal found about 1,400 duplicate customer rows; cleaning them means a second rehearsal. The forecast is the Data lead's single estimate; no range was given.

If nothing changes: Go-live (M2) moves from Mon 19 Jul to Mon 9 Aug, 15 working days late. Chain: UAT Mon 5 to Fri 16 Jul, training Mon 19 to Fri 23 Jul, cutover preparation Mon 26 to Fri 30 Jul. The next working day, Mon 2 Aug, is inside the Finance close (2 to 6 Aug, no go-live), so go-live moves to Mon 9 Aug. Later milestones: Hypercare ends (M3) Fri 20 Aug (10 working days counted from go-live day, as the settings say), 7 working days before the licence ends on Tue 31 Aug (M4, fixed). Dependencies hit: Vendor B on-site support is accepted for 19 to 20 Jul only; nothing is accepted for 9 Aug; the latest date to ask for a change is Mon 26 Jul (10 working days' notice). Already told the current date: Operations staff (Mon 19 Jul). No other audience is recorded.

Options: 4

Option 1: Defer the Reports module
- Change: UAT covers Booking and Invoicing only. Reports (Should, 3 working days, fallback stated) is deferred and gets no date. UAT falls from 10 to 7 working days.
- Takes out of the chain: 3 working days.
- Dates after: UAT Mon 5 to Tue 13 Jul; training Wed 14 to Tue 20 Jul; cutover preparation Wed 21 to Tue 27 Jul.
- Go-live: Wed 28 Jul, 7 working days after the committed date (8 fewer than if nothing changes).
- Later milestones: Hypercare ends Tue 10 Aug, 15 working days before the licence ends.
- Dependencies: Vendor B support for Wed 28 Jul not accepted; latest date to ask Wed 14 Jul.
- Rests on: the Data lead's 2 Jul date holding; the estimates for Booking and Invoicing holding; the fallback being acceptable (Finance makes the monthly report from the spreadsheet export, as done today).
- Costs: Reports has no date and needs its own decision. Finance makes the monthly report from the spreadsheet export until then.
- Confirm with: Test lead (UAT dates); Finance lead (the fallback, since the monthly report is Finance's).

Option 2: Start cutover preparation during training
- Change: cutover preparation starts 3 working days before training ends, that is on the third day of training.
- Takes out of the chain: 3 working days.
- Dates after: UAT Mon 5 to Fri 16 Jul; training Mon 19 to Fri 23 Jul; cutover preparation Wed 21 to Tue 27 Jul.
- Go-live: Wed 28 Jul, 7 working days after the committed date (8 fewer than if nothing changes).
- Later milestones: Hypercare ends Tue 10 Aug, 15 working days before the licence ends.
- Dependencies: Vendor B support for Wed 28 Jul not accepted; latest date to ask Wed 14 Jul.
- Rests on: the Operations lead's note that the first 3 working days (runbook, rollback plan, access list) do not need training to finish; UAT finishing on its forecast.
- Costs: None stated in the inputs.
- Confirm with: Operations lead (the overlap and dates); Training lead (training dates).

Option 3: Add one tester to UAT
- Change: the Support team tester joins UAT from Mon 5 Jul. R = 20, n = 2, k = 1, u = 3: (20 + 3) / 3 = 7.67, so 8 working days.
- Takes out of the chain: 2 working days.
- Dates after: UAT Mon 5 to Wed 14 Jul; training Thu 15 to Wed 21 Jul; cutover preparation Thu 22 to Wed 28 Jul.
- Go-live: Thu 29 Jul, 8 working days after the committed date (7 fewer than if nothing changes).
- Later milestones: Hypercare ends Wed 11 Aug, 14 working days before the licence ends.
- Dependencies: Vendor B support for Thu 29 Jul not accepted; latest date to ask Thu 15 Jul.
- Rests on: UAT dividing evenly across three testers (the Test lead marked it splittable); the newcomer adding nothing for 3 working days; the Support team lead releasing the tester (said "if asked"; nobody has asked); UAT starting on Mon 5 Jul as forecast.
- Costs: one Support tester, Mon 5 to Wed 14 Jul.
- Confirm with: Test lead (the split and the dates); Support team lead (release of the tester).

Option 4: Move go-live to Mon 9 Aug
- Change: no change to scope, order or people. Go-live is reset to Mon 9 Aug, the first allowed working day. The dates equal the do-nothing dates; the difference is that the commitment is re-baselined to Mon 9 Aug.
- Takes out of the chain: 0 working days.
- Dates after: UAT Mon 5 to Fri 16 Jul; training Mon 19 to Fri 23 Jul; cutover preparation Mon 26 to Fri 30 Jul.
- Go-live: Mon 9 Aug, 15 working days after the committed date (the same as if nothing changes).
- Later milestones: Hypercare ends Fri 20 Aug, 7 working days before the licence ends. The date holds if cutover preparation finishes by Fri 6 Aug, so it absorbs up to 5 working days of further slip.
- Dependencies: Vendor B support for Mon 9 Aug not accepted; latest date to ask Mon 26 Jul.
- Rests on: the Data lead's 2 Jul date holding; the Finance close staying 2 to 6 Aug.
- Costs: Operations staff were told Mon 19 Jul and would need a new date.
- Confirm with: Operations lead (dates); Finance lead (the close week).

Combinations: Options 1 and 2 together take out 6 working days: UAT Mon 5 to Tue 13 Jul; training Wed 14 to Tue 20 Jul; cutover preparation Fri 16 to Thu 22 Jul; go-live Fri 23 Jul, 4 working days after the committed date; hypercare ends Thu 5 Aug, 18 working days before the licence ends; Vendor B latest date to ask Fri 9 Jul. Options 1, 2 and 3 together take out 7 working days, not 8, because Options 1 and 3 act on the same task: Reports' 3 working days on 2 people are 6 person-days, so 14 remain, and (14 + 3) / 3 = 5.67, 6 working days. UAT Mon 5 to Mon 12 Jul; training Tue 13 to Mon 19 Jul; cutover preparation Thu 15 to Wed 21 Jul; go-live Thu 22 Jul, 3 working days after the committed date; hypercare ends Wed 4 Aug, 19 working days before the licence ends; Vendor B latest date to ask Thu 8 Jul. No combination restores Mon 19 Jul.

Not known: (1) Whether Finance accepts its 2 to 6 Aug close falling inside hypercare under Options 1 to 3; the inputs say only that go-live may not fall in it: Finance lead. (2) Whether Vendor B can support any date other than 19 to 20 Jul; nobody has asked: Operations lead. (3) Whether the Support team lead will release a tester: Support team lead. (4) Whether anyone other than Operations staff was told the current go-live date: project manager. (5) Whether any person is needed both in the first days of training and in the first 3 days of cutover preparation: Training lead and Operations lead.

Decision for the Managing director: choose one option or combination; the Test lead, Training lead and Operations lead confirm each date. Working days counted Monday to Friday; holidays used: none. Nothing is changed in the plan, promised to anyone or sent.
```

## What was observed

- Every part of the output format was produced and no stop condition applied. The page recommended nothing, drafted no message and changed no plan.
- The headline numbers match the example's: 10 working days late; go-live Mon 9 Aug (15 late) if nothing changes; Wed 28 Jul for the deferral and the overlap; Thu 29 Jul for the added tester; Fri 23 Jul for options 1 and 2; Thu 22 Jul for options 1, 2 and 3. I also recomputed these dates with a short script on a Monday-to-Friday calendar; they agree.
- The conversion rule closed the gap found in the first run: the Reports module's 3 working days on 2 people were taken as 6 person-days without a guess, giving 14 person-days and 6 working days for UAT.
- Every fact in the output is in the inputs or follows from the calendar. Every item under Not known carries an answerer. Where the inputs gave no answerer for the question about a shared person, I named the two leads whose tasks overlap.
- Differences from the published example: I could not make this run independent of it. The same session revised both, and I had the example's text in view, so the close agreement is not evidence that the instructions alone produce it. The differences are in wording only, not in dates: the run's dependency lines are shorter and omit "No request has been made"; the run omits the example's "hypercare covers Finance's close week" notes; it adds that hypercare is counted from go-live day, that UAT starts on Mon 5 Jul as forecast, and a note on why Options 1 and 3 overlap; it states the capacity formula's terms (R, n, k, u).
- Still open: the run was not repeated on another model, and the instruction block's sensitivity to a different set of inputs has not been tried. Stop conditions, the range forecast, the "not stated" cause, a missing export date and a passed latest-date-to-ask were not exercised by the example.
- This is one run, by one model, on one invented example. It is not a test for a client.

## What was changed after the earlier run

Changed on 10 November 2026 after the first run and an independent review (a read of the template and example by a reviewer who had not written them), and checked by the run recorded above:

- **Person-days.** The template now says how effort in working days becomes person-days: effort multiplied by the task's People Now when the items are done one after another, and ask if the note does not say so. A deferred item also shortens the task's duration by its effort in working days. Acceptance test 5 now states the conversion.
- **Inputs.** Today's date, the date of the schedule export, who was told the current date and who confirms deferrals are now named in the settings, and the example supplies them. The example's note now states that the monthly report is Finance's.
- **Claims the inputs did not support** were removed from the example: that Finance would "run its close on the new system", that the Operations and Training leads share no person, and that "no extra coordination time" is an assumption. The first two are now questions with answerers. Every Not known item names who can answer.
- **Wording.** Undefined terms are defined: "takes out of the chain" (days off the run of tasks, not the go-live saving), the overlap rule (N days of overlap starts on day duration minus N plus 1), which date the latest date to ask counts from (the first date the commitment is needed), that a settings rule for a milestone overrides the successor rule, and that a no-go period applies to the milestone it names.
- **Option order and the move-the-date option.** Options are numbered scope, resequence, capacity, move the date. When the moved date equals the do-nothing date the option says so and that it re-baselines the commitment.
- **The pasted instructions** now include the headline milestone exception, the "estimate not supplied" and "commitment and schedule disagree" exceptions, and the rules above.
- **Acceptance tests** 10 to 12 added.

## The earlier run, as recorded

This is the first run of 10 November 2026, on the template and example before the changes above. Its output and observations are unaltered.

### What came out

```
SCHEDULE RECOVERY OPTIONS: Migration rehearsal complete (M1)

For: Managing director. Dates to be confirmed by: Test lead, Training lead, Operations lead (Finance lead for any deferral that affects Finance). Prepared Wed 16 Jun 2027 from the schedule export of (date not stated).

The slip: M1 was committed for Fri 18 Jun and is now forecast for Fri 2 Jul, 10 working days late. Cause as reported: the migration rehearsal found about 1,400 duplicate customer rows; cleaning them means a second rehearsal. The forecast is the Data lead's single estimate.

If nothing changes: Go-live (M2) moves from Mon 19 Jul to Mon 9 Aug, 15 working days late. Chain: UAT Mon 5 to Fri 16 Jul, training Mon 19 to Fri 23 Jul, cutover preparation Mon 26 to Fri 30 Jul. The next working day, Mon 2 Aug, is inside the Finance close (2 to 6 Aug, no go-live), so go-live moves to Mon 9 Aug. Later milestones: Hypercare ends (M3) Fri 20 Aug, 7 working days before the licence ends on Tue 31 Aug (M4, fixed). Dependencies hit: Vendor B on-site support is accepted for 19 to 20 Jul only; nothing is accepted for 9 Aug; the latest date to ask for a change is Mon 26 Jul (10 working days' notice). Already told the current date: Operations staff (go-live, Mon 19 Jul), taken from the Committed To column.

Options: 4

Option 1: Defer the Reports module
- Change: UAT covers Booking and Invoicing only. Reports (Should, fallback stated) is deferred and gets no date.
- Takes out of the chain: 3 working days (UAT 10 to 7).
- Dates after: UAT Mon 5 to Tue 13 Jul; training Wed 14 to Tue 20 Jul; cutover preparation Wed 21 to Tue 27 Jul.
- Go-live: Wed 28 Jul, 7 working days after the committed date (8 fewer than if nothing changes).
- Later milestones: Hypercare ends Tue 10 Aug, 15 working days before the licence ends.
- Dependencies: Vendor B support for 28 Jul not accepted; latest date to ask Wed 14 Jul.
- Rests on: the Data lead's 2 Jul date holding; the estimates for Booking and Invoicing holding; the fallback (monthly report from the spreadsheet export, as done today) being acceptable.
- Costs: Reports has no date and needs its own decision. Nothing else stated in the inputs.
- Confirm with: Test lead (UAT dates); Finance lead (the fallback, if the deferral affects Finance).

Option 2: Add one tester to UAT
- Change: the Support team tester joins UAT from Mon 5 Jul. R = 20, n = 2, k = 1, u = 3: (20 + 3) / 3 = 7.67, so 8 working days.
- Takes out of the chain: 2 working days.
- Dates after: UAT Mon 5 to Wed 14 Jul; training Thu 15 to Wed 21 Jul; cutover preparation Thu 22 to Wed 28 Jul.
- Go-live: Thu 29 Jul, 8 working days after the committed date (7 fewer than if nothing changes).
- Later milestones: Hypercare ends Wed 11 Aug, 14 working days before the licence ends.
- Dependencies: Vendor B support for 29 Jul not accepted; latest date to ask Thu 15 Jul.
- Rests on: UAT being splittable as the Test lead marked it; the newcomer adding nothing for 3 working days; the tester being released (Support team lead said "if asked"; nobody has asked).
- Costs: one Support tester, Mon 5 to Wed 14 Jul.
- Confirm with: Test lead (the split and the dates); Support team lead (release of the tester).

Option 3: Start cutover preparation during training
- Change: cutover preparation starts 3 working days before training ends, on the third day of training.
- Takes out of the chain: 3 working days.
- Dates after: UAT Mon 5 to Fri 16 Jul; training Mon 19 to Fri 23 Jul; cutover preparation Wed 21 to Tue 27 Jul.
- Go-live: Wed 28 Jul, 7 working days after the committed date (8 fewer than if nothing changes).
- Later milestones: Hypercare ends Tue 10 Aug, 15 working days before the licence ends.
- Dependencies: Vendor B support for 28 Jul not accepted; latest date to ask Wed 14 Jul.
- Rests on: the Operations lead's note that the first 3 working days (runbook, rollback plan, access list) do not need training to finish; UAT finishing on its forecast.
- Costs: None stated in the inputs.
- Confirm with: Operations lead (the overlap and dates); Training lead (training dates).

Option 4: Move go-live to Mon 9 Aug
- Change: no change to scope, order or people. Go-live is reset to Mon 9 Aug, the first allowed working day.
- Takes out of the chain: 0 working days.
- Dates after: UAT Mon 5 to Fri 16 Jul; training Mon 19 to Fri 23 Jul; cutover preparation Mon 26 to Fri 30 Jul.
- Go-live: Mon 9 Aug, 15 working days after the committed date (the same as if nothing changes).
- Later milestones: Hypercare ends Fri 20 Aug, 7 working days before the licence ends. The date holds if cutover preparation finishes by Fri 6 Aug, so it absorbs up to 5 working days of further slip.
- Dependencies: Vendor B support for 9 Aug not accepted; latest date to ask Mon 26 Jul.
- Rests on: the Data lead's 2 Jul date holding; the Finance close staying 2 to 6 Aug.
- Costs: Operations staff were told 19 Jul and would need a new date. Scope is kept.
- Confirm with: Operations lead (dates).

Combinations: Options 1, 2 and 3 together take out 7 working days, not 8, because 1 and 2 act on the same task: with Reports gone UAT is 14 person-days, so (14 + 3) / 3 = 5.67, 6 working days. UAT Mon 5 to Mon 12 Jul; training Tue 13 to Mon 19 Jul; cutover preparation Thu 15 to Wed 21 Jul; go-live Thu 22 Jul, 3 working days after the committed date; hypercare ends Wed 4 Aug, 19 working days before the licence ends; Vendor B latest date to ask Thu 8 Jul. Options 2 and 3 together (no scope given up): UAT Mon 5 to Wed 14 Jul; training Thu 15 to Wed 21 Jul; cutover preparation Mon 19 to Fri 23 Jul; go-live Mon 26 Jul, 5 working days after the committed date; hypercare ends Fri 6 Aug, 17 working days before the licence ends; Vendor B latest date to ask Mon 12 Jul. No combination restores Mon 19 Jul.

Not known: (1) Whether the Reports deferral affects Finance: Finance lead. (2) Whether Vendor B can support any date other than 19 to 20 Jul: nobody has asked; Operations lead. (3) Whether the Support team lead will release a tester: Support team lead. (4) Whether the Test lead agrees UAT can be split across a third tester when the modules are tested one after another: Test lead. (5) Whether anyone other than Operations staff was told the current go-live date: project manager.

Decision for the Managing director: choose one option or combination; the Test lead, Training lead and Operations lead confirm each date. Working days counted Monday to Friday; holidays used: none. Nothing is changed in the plan, promised to anyone or sent.
```

### What the earlier run observed

- Every required part of the output format was produced, and no stop condition was triggered: all headers matched, all predecessors exist, the forecast is later than the commitment and a calendar was supplied. The assistant did not recommend, did not draft a message and did not change the plan.
- The headline numbers match the published example: 10 working days late, go-live Mon 9 Aug (15 late) if nothing changes, Wed 28 Jul for the deferral and the overlap, Thu 29 Jul for the added tester, and Thu 22 Jul for the three together.
- Differences from the published example:
  - Option order differs (I put the added tester second, the overlap third). The template does not fix an order.
  - I gave the second combination as options 2 and 3 (no scope given up). The example gives options 1 and 2. The template leaves the choice open.
  - I gave a latest date to ask Vendor B in the do-nothing case (Mon 26 Jul), as the example does; the procedure asks for it only for options.
  - I wrote "(date not stated)" for the schedule export date. The example says "that date". The inputs do not give the export's date.
  - The example's rests-on and costs lines include things the inputs do not say: that the Operations and Training leads share no person, that Finance "keeps the manual report", and that Finance would need to run its close on the new system. I left these out or turned them into questions.
- Where the instructions were ambiguous and I had to choose:
  1. "Takes out of the chain" is not defined. I used working days off the chain of tasks, not days off the go-live date, which also includes the days saved by avoiding the Finance close.
  2. The scope list gives effort in working days; the capacity formula uses person-days. To remove the Reports module from a task with two people I took 3 working days as 6 person-days, from the note that the modules run one after another over 10 days with 2 people. The template does not say how to convert. Taking 3 person-days instead would give a different combined result (go-live Fri 23 Jul).
  3. The procedure says a task starts the working day after its predecessor, but the hypercare milestone (M3) sits 9 working days after go-live in the schedule. I used the settings' rule ("10 working days counted from go-live day") and did not apply the Finance no-go period to hypercare, because the no-go is stated for go-live only. The template does not say either.
  4. "May start N working days before its predecessor ends" can be read as starting on the third-from-last day or three days before that. I read it as starting on the third day of a five-day task (so three days overlap), which matches acceptance test 4.
  5. "Already told the current date" is not an input. I took the Committed To column as the audience, which is a guess.
  6. The settings are said to include "today's date", and the output asks for the date of the schedule export; the example supplies neither as a labelled field.
  7. The tester is marked splittable, but the note says the three modules are tested one after another. The formula assumes the work divides evenly. I applied it and flagged it as a question for the Test lead.
  8. "Move the date" gives the same result as doing nothing here, because the no-go period has already moved go-live. I offered it as the fourth option, with the amount of further slip it absorbs (5 working days), but it is not a real alternative in this case.
  9. The acceptance tests refer to options by number (for example "Options 1, 2 and 3 together"), but the template does not fix the order of options.
  10. When computing the latest date to ask a supplier, I used the new go-live date minus the notice. The template says "the new date" without saying whether that is go-live or the start of support.
- No fact in my output is missing from the inputs, apart from the two guesses above (the audience and the preparation date) and the working-day counts, which follow from the calendar.
- This is one run, by one model, on one invented example. It shows the instructions can be followed to a page that matches the published one on dates. It is not a test for a client.

