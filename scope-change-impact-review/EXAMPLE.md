# Scope change impact review: an invented example

*Illustrative example with invented data.* The firm, its people, the project and every date and figure below are invented. The firm is an invented 70-person accounting and advisory firm building a client portal, where clients upload documents, see where their work stands and book time with an adviser. The project manager runs the project, the operations director sponsors it and the portal lead estimates the work; people are named by role only. On Tuesday 10 November 2026 the project manager supplied the seven inputs below, in full, and got back the review that follows.

## The inputs

### 1. Settings

```
Project: Client portal
Sponsor: Operations director
Project manager: Project manager
Approvers of changes: Operations director
Delivery lead (gives estimates): Portal lead
Day rate: $650 a day, blended
Working days: Monday to Friday
Closed days: Thursday 24 December 2026 to Friday 1 January 2027
Review date: Tuesday 10 November 2026
```

### 2. Baseline facts

```
Approved: Monday 14 September 2026, by the Operations director
End date: Friday 4 December 2026
Effort: 55 days
Budget: $39,750 (55 days at $650 = $35,750, plus $4,000 for the
  portal licence)
Excluded from scope:
- Online payment of invoices by card
- Pages in languages other than English
- A mobile app
```

### 3. Baseline deliverables

```
Ref,Deliverable,Due,Effort days
D1,Portal design and page templates agreed,2026-10-02,6
D2,Client document upload and download,2026-10-23,12
D3,Client sign-in and account set-up,2026-11-13,18
D4,Engagement status page,2026-11-06,5
D5,Migration of 40 help articles,2026-11-20,8
D6,Launch and client invitation emails,2026-12-04,6
```

### 4. Working list (exported from the project tracker on 10 November)

```
Ref,Deliverable,Due,Status
D1,Portal design and page templates agreed,2026-10-02,Done
D2,Client document upload and download,2026-10-23,Done
D3,Client sign-in and account set-up,2026-11-13,In progress
D4,Engagement status page,2026-11-06,Done
D5,Migration of 55 help articles,2026-11-20,In progress
D6,Launch and client invitation emails,2026-12-11,Not started
A1,Appointment booking with advisers,2026-11-27,Not started
A2,Document request checklist for each client,2026-11-25,In progress
A3,Card payment of invoices,2026-11-30,Not started
A4,Pages in Spanish,2026-12-02,Not started
A5,Saved favourite documents,2026-11-27,Not started
```

### 5. Change log

```
Change,Ref,Description,Decision,Decided by,Decided on,Effort days,Other cost,End date after
CR-01,A1,Appointment booking with advisers,Approved,Operations director,2026-10-16,7,1200,2026-12-11
CR-02,A4,Pages in Spanish,Declined,Operations director,2026-10-30,,,
```

### 6. Request notes

```
Weekly portal meeting, Thursday 22 October 2026 (notes by the project
manager)
- The tax manager asked for a checklist on each client's page showing
  which documents we still need from them. Portal lead: "Should be
  fine, we'll fit it in." Added to the plan as A2.
- The audit partner asked whether the portal could print a summary of
  each client's open requests. Not discussed further.

Email, Monday 2 November 2026, from the finance director to the
project manager
"Clients keep asking to pay our invoices by card. Can the portal take
card payments before launch?"

Email, Wednesday 4 November 2026, from the content lead to the portal
team
"The tax and advisory teams sent 15 more help articles they want moved
across, so I've changed the migration to 55 articles."
```

### 7. Estimates (from the portal lead, Monday 9 November)

```
Ref,Effort days,Other cost,End date effect,Estimated by,Assumptions
D5,3,0,0,Portal lead,15 more articles at the same pace as the first 40; fits before launch
A2,9,2400,5,Portal lead,"Needs the portal's reminder add-on, $2,400 for a year"
A3,11,1800,10,Portal lead,"Card payment provider's set-up fee, $1,800; finance opens the provider account"
```

## The output

```
SCOPE CHANGE IMPACT REVIEW: Client portal, as of Tuesday 10 November 2026
DRAFT for the Project manager. The Operations director accepts or declines each change.

For: Operations director. Baseline approved Monday 14 September 2026 by the Operations director. Approvers of changes: Operations director.
Compared: 6 baseline deliverables; 11 rows in the working list; 2 change-log rows; request notes: the weekly portal meeting notes of 22 October and two emails; estimates for 3 of 4 pending changes.

POSITION
Baseline: 6 deliverables, 55 days, $39,750, end date Friday 4 December 2026.
Approved changes: 1 (CR-01): +7 days, +$5,750. Now 62 days, $45,500, end date Friday 11 December 2026.
Pending changes: 4: +23 days, +$19,150 for those estimated; not estimated: A5. If all were accepted: 85 days, $64,650, plus A5, not estimated. End dates are shown for each change alone and are not added together.

WORK STARTED WITHOUT APPROVAL: 2
D5 Migration of 55 help articles. Status: In progress. Due in the working plan 20 November.
A2 Document request checklist for each client. Status: In progress. Due in the working plan 25 November.

DECISIONS FOR THE OPERATIONS DIRECTOR: 4
1. Accept or decline D5 Migration of 55 help articles, changed from the baseline "Migration of 40 help articles"?
   Asked for by: the content lead, for the tax and advisory teams, 4 November (email to the portal team).
   Status: In progress, work started without approval.
   Effect: 3 days; $1,950 (3 days at $650, no other cost); end date Friday 11 December 2026 if accepted alone (no change), per the Portal lead.
   Assumptions: 15 more articles at the same pace as the first 40; fits before launch.
   In the working plan for: 20 November.
2. Accept or decline A2 Document request checklist for each client?
   Asked for by: the tax manager, 22 October (weekly portal meeting notes). Agreed in the notes by the Portal lead, who is not an approver; that is not an approval.
   Status: In progress, work started without approval.
   Effect: 9 days; $8,250 (9 days at $650, plus $2,400 other); end date Friday 18 December 2026 if accepted alone (+5 working days), per the Portal lead.
   Assumptions: Needs the portal's reminder add-on, $2,400 for a year.
   In the working plan for: 25 November.
3. Accept or decline A5 Saved favourite documents?
   Asked for by: not found.
   Status: Not started.
   Effect: not estimated.
   Assumptions: none given.
   In the working plan for: 27 November.
4. Accept or decline A3 Card payment of invoices?
   Asked for by: the finance director, 2 November (email to the project manager).
   Status: Not started.
   Effect: 11 days; $8,950 (11 days at $650, plus $1,800 other); end date Tuesday 5 January 2027 if accepted alone (+10 working days, skipping closed days), per the Portal lead.
   Assumptions: Card payment provider's set-up fee, $1,800; finance opens the provider account.
   Appears to match the baseline exclusion "Online payment of invoices by card".
   In the working plan for: 30 November.

COMPARISON WITH THE BASELINE
Unchanged: 4 of 6 baseline deliverables (D1, D2, D3, D4).
Approved additions and changes: A1 Appointment booking with advisers, CR-01, Operations director, 16 October.
Not approved: D5 (changed wording), no change-log entry; A2, no change-log entry; A3, no change-log entry; A5, no change-log entry.
Declined but still in the working plan: A4 Pages in Spanish, CR-02, Operations director, 30 October.
Dates moved: D6 Launch and client invitation emails, from 4 December to 11 December; not later than the current end date.
Baseline deliverables not in the working list: none.
Approved changes not in the working list: none.
Requests in the notes not in the working list: a printable summary of each client's open requests, the audit partner, 22 October (weekly portal meeting notes).

FOR THE PROJECT MANAGER ONLY. Remove before sharing.
Questions: 6
1. D5 Migration of 55 help articles is in progress without an approved change. Does the extra work carry on while the Operations director decides?
2. A2 Document request checklist for each client is in progress without an approved change. Does the work carry on while the Operations director decides?
3. A4 Pages in Spanish was declined by the Operations director on 30 October (CR-02) and is still in the working plan. Does it come out of the plan, or go back to the Operations director?
4. A5 Saved favourite documents has no request in the notes and no estimate. Who asked for it, and will the Portal lead estimate it before the Operations director decides?
5. A3 Card payment of invoices appears to match the baseline exclusion "Online payment of invoices by card". Is it the same work?
6. The audit partner asked on 22 October for a printable summary of each client's open requests. It is not in the working list or the change log. Does it go to the Operations director as a change?
Prepared for the Project manager. Nothing has been accepted, declined, added to or removed from the plan, estimated, or sent.
```

## How the figures were reached

- **Baseline:** 6 + 12 + 18 + 5 + 8 + 6 = 55 days, matching the stated total, so the review went ahead.
- **Approved change CR-01:** 7 days at $650 = $4,550, plus $1,200 other = $5,750. Now 55 + 7 = 62 days and $39,750 + $5,750 = $45,500. The end date is CR-01's agreed date, Friday 11 December 2026.
- **D5:** 3 × $650 = $1,950. **A2:** 9 × $650 = $5,850, plus $2,400 = $8,250; five working days after Friday 11 December is Friday 18 December. **A3:** 11 × $650 = $7,150, plus $1,800 = $8,950; ten working days after Friday 11 December, with the office closed from 24 December to 1 January, run 14 to 18 December, 21 to 23 December, then 4 and 5 January, so Tuesday 5 January 2027.
- **Pending totals:** 3 + 9 + 11 = 23 days and $1,950 + $8,250 + $8,950 = $19,150. If all were accepted, 62 + 23 = 85 days and $45,500 + $19,150 = $64,650, before A5.
- **Order of decisions:** D5 (in progress, due 20 November) and A2 (in progress, due 25 November) come first; then A5 (27 November) and A3 (30 November).
- **D6** moved to 11 December, the same day as the current end date, so it is listed but raises no question. **A4** was declined, so it gets a question for the project manager rather than a decision. **A1** is approved and in the plan, so it raises nothing.

The project manager answers the six questions, removes the last part and takes the decisions to the operations director. The review changed nothing in the plan or the change log and sent nothing.
