# Sprint plan against capacity: an invented example

*Illustrative example with invented data.* The company, the team, the people, the items and every figure below are invented. The company is an invented 60-person business that sells appointment-booking software; its booking team works in two-week sprints. People are named by role and letter only. The delivery lead prepared the draft on the Friday the ending sprint closed, for the planning meeting the following Monday. First come the five inputs the delivery lead supplied, in full, then the draft the workflow template returned.

## The inputs

### 1. Settings

```
Team: Booking team
Iteration being planned: Sprint 25, Monday 16 November 2026 to Friday 27 November 2026
Iteration ending: Sprint 24
Working days: Monday to Friday
Closed days: Thursday 26 and Friday 27 November 2026 (company holiday)
Estimate unit: points
Done statuses: Done
Ready statuses: Ready
Plan to: the average
Planning meeting: Monday 16 November 2026
Board exported: Friday 13 November 2026
```

### 2. Board export

```
Key,Title,Status,Estimate,Remaining,Rank,Assignee,Iteration,Depends on
APP-305,Recurring appointments: data model,Done,5,0,,Dev A,Sprint 24,
APP-311,Export appointments to a spreadsheet file,In progress,5,3,4,Dev A,Sprint 24,
APP-318,Fix reminder emails sent twice,In review,3,,2,Dev B,Sprint 24,
APP-320,Recurring appointments: weekly pattern,Ready,8,,1,Dev A,Sprint 25,APP-305
APP-322,Recurring appointments: change one occurrence,Ready,5,,3,Dev C,Sprint 25,APP-320
APP-325,Two-way calendar sync,Ready,8,,5,Dev B,,PAY-88
APP-327,Notes field on an appointment,Ready,3,,6,Dev C,,
APP-329,Accessibility fixes on the booking page,To refine,,,7,,,
APP-331,Reminder settings page redesign,Ready,5,,8,Designer,,APP-333
APP-333,Reminder settings service,Ready,3,,9,Dev A,,
APP-335,Bulk cancel appointments,Ready,5,,10,Dev C,,
APP-340,Waiting list for full days,Ready,8,,11,,Sprint 26,
```

### 3. Team availability

```
Person,Role,Allocation,Days out
Dev A,Developer,100%,
Dev B,Developer,100%,2026-11-19;2026-11-20
Dev C,Developer,50%,
Tester,Tester,100%,2026-11-27
Designer,Designer,50%,
```

### 4. Recent delivery

```
Iteration,Person-days,Committed,Completed
Sprint 22,36.0,40,36
Sprint 23,40.0,42,34
Sprint 24,32.0,36,30
```

### 5. The product owner's notes

```
Goal: Customers can book an appointment that repeats every week.
Must include: APP-320, APP-322.
Held back: APP-335, until support's feedback is in.
```

## The draft the workflow template returned

**SPRINT PLAN AGAINST CAPACITY: Booking team, Sprint 25, Monday 16 November 2026 to Friday 27 November 2026**

Draft for the planning meeting on Monday 16 November 2026. Board exported Friday 13 November 2026. The team decides the commitment.
Board rows: 12 read; 1 done; 1 in another iteration, not considered.

**Capacity**

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

**Carryover from Sprint 24: 2 items, 6 points.**

- APP-318 Fix reminder emails sent twice: status In review, estimate 3, size this iteration 3 (remaining not stated, full estimate used). Assignee Dev B.
- APP-311 Export appointments to a spreadsheet file: status In progress, estimate 5, size this iteration 3. Assignee Dev A.

**Draft plan, in order**

1. APP-318 Fix reminder emails sent twice (carried): 3. Running total 3. Assignee Dev B. Waits on nothing.
2. APP-311 Export appointments to a spreadsheet file (carried): 3. Running total 6. Assignee Dev A. Waits on nothing.
3. APP-320 Recurring appointments: weekly pattern: 8. Running total 14. Assignee Dev A. Waits on APP-305, done.
4. APP-322 Recurring appointments: change one occurrence: 5. Running total 19. Assignee Dev C. Waits on APP-320, earlier in this draft.
5. APP-325 Two-way calendar sync: 8. Running total 27. Assignee Dev B. Waits on PAY-88, outside the export, status unknown.

--- Planning line: 27 of 27 points planned; 0 left under the planning figure.

Below the line, in order:

6. APP-327 Notes field on an appointment: 3. Waits on nothing.
7. APP-331 Reminder settings page redesign: 5. Waits on APP-333, later in the order, both below the line.
8. APP-333 Reminder settings service: 3. Waits on nothing.

Set aside:

- APP-329 Accessibility fixes on the booking page: not ready: To refine; no estimate.
- APP-335 Bulk cancel appointments: held back by the product owner.

**What items wait on**

- APP-320 waits on APP-305: done.
- APP-322 waits on APP-320: earlier in this draft.
- APP-325 waits on PAY-88: outside the export, status unknown.
- APP-331 waits on APP-333: later in the order, both below the line.

**Product owner's notes against the draft**

Goal: Customers can book an appointment that repeats every week.
Must include: APP-320: above the line. APP-322: above the line.
Held back: APP-335.

**Load by person**

- Dev A: 8.0 person-days. Above the line: APP-311, APP-320 (11 points).
- Dev B: 6.0 person-days, out Thursday 19 and Friday 20 November. Above the line: APP-318, APP-325 (11 points).
- Dev C: 4.0 person-days. Above the line: APP-322 (5 points).
- Tester: 8.0 person-days, out Friday 27 November (closed day, not counted). Nothing assigned.
- Designer: 4.0 person-days. Nothing assigned.
- Unassigned above the line: none.

Points measure the team's work, not one person's; no comparison is made.

**Assumptions**

1. Allocations and days out are as supplied: Dev C and the Designer give 50% of their time to this team.
2. The Tester's day out on Friday 27 November falls on a closed day and is not counted.
3. The forecast uses the last three sprints: 100 points completed over 108.0 person-days, times 30.0 person-days, rounded down.
4. APP-318 has no remaining size; its full estimate of 3 points is used.
5. APP-325 is counted as if PAY-88, which is not on this board, will be ready in time.

**Questions for the team**

1. APP-318 is in review and its remaining size is not stated. How much of its 3 points is left?
2. APP-325 (8 points) waits on PAY-88, which is not in this export. Will PAY-88 be ready in time? If not, APP-325 comes out and 8 points are free under the planning figure.
3. Dev B is out on Thursday 19 and Friday 20 November and is assigned APP-318 and APP-325 above the line. Does that assignment hold?
4. APP-329 is in To refine with no estimate. Is it refined and estimated before planning, or left for a later sprint?
5. APP-331 waits on APP-333, which comes after it in the order. If either is brought above the line, does APP-333 come first, or both together?
6. The draft totals 27 points, the forecast. At the lowest past rate, 0.85, the forecast would be 25, which is 2 points fewer. Does the team commit to all 27?

Every figure traces to the board export of Friday 13 November 2026, the availability sheet and the delivery history supplied. Nothing on the board has been changed, assigned or committed.
