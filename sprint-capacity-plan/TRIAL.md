# Trial: Sprint plan against capacity, run once on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-11

The inputs were the invented example in `public/example.md` (the settings, board export, team availability, recent delivery and the product owner's notes). No client data was used. I did not write the template. I followed its instruction block and output format on those inputs, then compared the result with the published example output and the reviewer checklist.

One limit on this trial: the example file holds its inputs and its output together, and my first read of it showed both. So I did not produce my draft blind. I worked every figure out again from the inputs, and I treat the match with the published output as a check of the arithmetic, not as independent proof that the instructions lead to it.

## What came out

**SPRINT PLAN AGAINST CAPACITY: Booking team, Sprint 25, Monday 16 November 2026 to Friday 27 November 2026**

Draft for the planning meeting on Monday 16 November 2026. Board exported Friday 13 November 2026. The team decides the commitment.
Board rows: 12 read; 1 done; 1 in another iteration, not considered.

Capacity
Working days: 8. Skipped: Saturday 21 and Sunday 22 November; Thursday 26 and Friday 27 November (closed).
- Dev A, Developer: 8 working days, 0 days out, allocation 100%, 8.0 person-days.
- Dev B, Developer: 8 working days, 2 days out, allocation 100%, 6.0 person-days.
- Dev C, Developer: 8 working days, 0 days out, allocation 50%, 4.0 person-days.
- Tester, Tester: 8 working days, 0 days out (the day out on Friday 27 November is a closed day, not counted), allocation 100%, 8.0 person-days.
- Designer, Designer: 8 working days, 0 days out, allocation 50%, 4.0 person-days.

Person-days available: 30.0.
Recent delivery:
- Sprint 22: completed 36 of 40 committed, 36.0 person-days, rate 1.00.
- Sprint 23: completed 34 of 42 committed, 40.0 person-days, rate 0.85.
- Sprint 24: completed 30 of 36 committed, 32.0 person-days, rate 0.94.

Average rate: 0.93 per person-day (lowest 0.85, highest 1.00).
Forecast: 27 points (range 25 to 30).
Planning figure: 27 points, the forecast.

Carryover from Sprint 24: 2 items, 6 points.
- APP-318 Fix reminder emails sent twice: status In review, estimate 3, size this iteration 3 (remaining not stated, full estimate used). Assignee Dev B.
- APP-311 Export appointments to a spreadsheet file: status In progress, estimate 5, size this iteration 3. Assignee Dev A.

Draft plan, in order
1. APP-318 Fix reminder emails sent twice (carried): 3. Running total 3. Assignee Dev B. Waits on nothing.
2. APP-311 Export appointments to a spreadsheet file (carried): 3. Running total 6. Assignee Dev A. Waits on nothing.
3. APP-320 Recurring appointments: weekly pattern: 8. Running total 14. Assignee Dev A. Waits on APP-305 (done).
4. APP-322 Recurring appointments: change one occurrence: 5. Running total 19. Assignee Dev C. Waits on APP-320 (earlier in this draft).
5. APP-325 Two-way calendar sync: 8. Running total 27. Assignee Dev B. Waits on PAY-88 (outside the export, status unknown).
--- Planning line: 27 of 27 points planned; 0 left under the planning figure.
Below the line, in order:
6. APP-327 Notes field on an appointment: 3. Waits on nothing.
7. APP-331 Reminder settings page redesign: 5. Waits on APP-333 (later in the order, both below the line).
8. APP-333 Reminder settings service: 3. Waits on nothing.
Set aside:
- APP-329 Accessibility fixes on the booking page: not ready: To refine; no estimate.
- APP-335 Bulk cancel appointments: held back by the product owner.

What items wait on
- APP-320 waits on APP-305: done.
- APP-322 waits on APP-320: earlier in this draft.
- APP-325 waits on PAY-88: outside the export, status unknown.
- APP-331 waits on APP-333: later in the order, both below the line.

Product owner's notes against the draft
Goal: Customers can book an appointment that repeats every week.
Must include: APP-320: above the line. APP-322: above the line.
Held back: APP-335 (set aside).

Load by person
- Dev A: 8.0 person-days. Above the line: APP-311, APP-320 (11 points).
- Dev B: 6.0 person-days, out 2026-11-19 and 2026-11-20. Above the line: APP-318, APP-325 (11 points).
- Dev C: 4.0 person-days. Above the line: APP-322 (5 points).
- Tester: 8.0 person-days, day out 2026-11-27 (closed day, not counted). Nothing assigned.
- Designer: 4.0 person-days. Nothing assigned.
- Unassigned above the line: none.
Points measure the team's work, not one person's; no comparison is made.

Assumptions
1. Allocations and days out are as supplied. Dev C and the Designer give 50% of their time to this team.
2. The Tester's day out on Friday 27 November falls on a closed day and is not counted.
3. The forecast is total completed over total person-days (100 over 108.0 = 0.9259), times 30.0 person-days (27.78), rounded down to 27. The range is 0.85 times 30.0 (25.5, rounded down to 25) to 1.00 times 30.0 (30).
4. APP-318 has a blank Remaining; it is treated as not stated and its full estimate of 3 is used.
5. APP-325 is counted as if PAY-88, which is not in the export, will be ready in time.
6. APP-305 is done and so is not carried. APP-340 is in Sprint 26 and is not considered.

Questions for the team
1. APP-318 is in review and its remaining size is not stated. How much of its 3 points is left?
2. APP-325 (8 points) waits on PAY-88, which is not in the export. Will PAY-88 be ready in time? If not, APP-325 comes out and 8 points are free under the planning figure of 27 (the plan would total 19).
3. Dev B is out on 19 and 20 November (6.0 person-days) and is assigned APP-318 and APP-325 above the line, 11 points. Does that assignment hold?
4. APP-329 is in To refine with no estimate. Is it refined and estimated before planning, or left for a later sprint?
5. APP-331 waits on APP-333, which is later in the order; both are below the line. If either is brought above the line, does APP-333 come first, or both together?
6. The draft totals 27 points, the forecast. At the lowest past rate (0.85) the forecast is 25, 2 points fewer. Does the team commit to all 27?

Every figure traces to the board export of Friday 13 November 2026, the availability sheet and the delivery history supplied. Nothing on the board has been changed, assigned or committed.

## What was observed

- Every required part of the output format was produced, and nothing in the procedure sent me to stop. No heading mismatch, duplicate key, missing allocation or missing input arose. The stop conditions were therefore not exercised.
- The figures agree with the published example: 8 working days, 30.0 person-days, rates 1.00, 0.85 and 0.94, average 0.93, forecast 27 (range 25 to 30), carryover 6 points, line after APP-325 at exactly 27, and the same items below the line and set aside.
- Differences from the published example are small. Mine states the Tester's day out in the load list and in the capacity list. It adds assumption 3's working in full and an assumption about APP-305 and APP-340. It says in question 2 what the plan would total if APP-325 came out. The example's questions run in the same order and cover the same points.
- Nothing in either output is a fact absent from the inputs. Both derive every name, key, date and figure from them. The example's wording "if either is brought above the line, does APP-333 come first, or both together" is a suggestion for the team, not a fact.
- Where I had to judge, the template was ambiguous in these places:
  - A blank `Remaining` cell on one row, when the column exists. The template covers a missing column, not a blank cell. I read a blank as "not stated". A `Remaining` of 0 on an item that is not done is also not covered.
  - Whether weekends inside the iteration count as "skipped" dates to list. The format example only mentions "closed" days. I listed them, as the published example does.
  - Whether to show a day out that falls on a closed day in the load list. The format says "out dates"; I showed it and marked it not counted.
  - What to do with a below-the-line item that waits on a set-aside item. The procedure checks dependencies only while drawing the line. The example here did not raise it.
  - Whether the "done" row and the "another iteration" row can overlap in the counts at the top. They did not here.
  - The format line for each past iteration reads "completed [n] of [n] committed", which is clear, but the average rate line shows two decimals while the working uses four. I added the working to the assumptions to make it checkable.
- This trial covers the ordinary path only. The template's twelve proposed acceptance tests (renamed heading, no history, circular dependencies, a request to commit or to compare people, and so on) were not run here.

## After the run

Notes added by an editor after the trier finished, not observations from the run.

- The template's version note, which said it had not been tried on its invented example, was out of date and has been updated.
- After an independent review, small edits followed to the template, the profile and the example's question 6 wording, and later to the wording about blank cells, days out on closed days and the order of the draft. The trial's output above was not changed. The example now shows the Tester's closed-day absence inline, as this run did. The edits were not re-run.
- A later review pass changed the template only in wording and numbering (the range now states that it uses the unrounded rates, the instruction block's steps are numbered as the procedure's are, and the settings note says which choices need a block edit), and the example only in one punctuation mark. No figure or output changed and the run was not repeated. The trial's output above is as recorded.
