# Project lessons review: an invented example

*Illustrative example with invented data.* The firm, its people, its clients, its supplier, the project and every date and figure below are invented. The firm is an invented 45-person accounting firm that has just finished the first phase of moving client documents from email to a secure client portal. The practice manager ran the project for the managing partner; the delivery leads were the IT lead, the client services manager and the tax manager. People are named by role only, and the portal supplier is called Vendor A. First come the six inputs the practice manager supplied, in full, then the draft the workflow template returned.

## The inputs

### 1. The review brief

```
Project: Client document portal
Phase reviewed: Phase 1, set-up and tax clients
Review date: 2026-11-12
Project manager: Practice manager
Sponsor: Managing partner
Delivery leads: IT lead; Client services manager; Tax manager
Aims:
  A1 Tax clients send their documents through the portal instead of by email.
  A2 Staff spend less time chasing missing documents.
  A3 Client files are complete before tax preparation starts.
Planned start: 2026-06-01
Planned finish: 2026-09-25
Actual finish: 2026-10-16
Baseline budget: $48,000
Actual cost: $55,300
Days: calendar
```

### 2. The deliverables list (exported from the project tracker)

```
ID,Deliverable,In original scope,Outcome,Change ref
D1,Portal set up with the firm's client folders and logo,yes,delivered,
D2,Portal accounts for all 400 tax clients,yes,delivered,
D3,Client how-to guide and two-minute video,yes,delivered,
D4,Electronic signature for tax return authorisation forms,yes,deferred,C2
D5,Portal accounts for 120 bookkeeping clients,no,delivered,C1
D6,Three staff training sessions,yes,delivered,
D7,Automatic reminders to clients with missing documents,yes,partly delivered,
```

### 3. The change log

```
Ref,Date,Change,Type,Days effect,Cost effect,Reason,Approved by
C1,2026-07-08,Add the 120 bookkeeping clients to phase 1,scope,14,6000,The partners asked for bookkeeping clients to join before year end,Managing partner
C2,2026-08-19,Move electronic signature to phase 2,scope,-7,-2500,Vendor A's signature module is not available in our region until January,Managing partner
C3,2026-09-02,Extra data-cleaning days for client email addresses,schedule,7,1800,Duplicate and out-of-date client email addresses found when invitations bounced,
```

### 4. The success measures

```
ID,Measure,Aim,Better,Starting value,Target,Fail level,Actual,As of,Result due,Source
M1,Tax clients who have uploaded through the portal at least once (%),A1,higher,0,70,,58,2026-11-06,,Portal usage report
M2,Client documents received by email in October,A1,lower,1850,300,600,240,2026-10-31,,Email intake log
M3,Staff hours a week spent chasing missing documents,A2,lower,,20,35,,,2026-12-11,Timesheets (new code from 2 November)
M4,Tax client portal accounts created,A1,higher,0,400,350,400,2026-09-18,,Portal admin report
```

### 5. The lessons notes (from the lessons session on 10 November)

```
PRACTICE MANAGER (project manager)
- Worked: nothing to add beyond the others.
- Didn't work: Vendor A's demo showed electronic signature, and we put
  it in scope without asking whether it worked in our region. It
  didn't (C2).
- Change I propose: before any feature goes into scope, the IT lead
  gets written confirmation from the vendor that it is available for
  our account and region. Owner: IT lead. Follow-up date: not agreed
  yet.
- On the measures: M4 counted accounts we created, which tells us
  nothing about whether clients use the portal. And M1 never got a
  fail level.
- Change I propose: before work starts, the project manager records a
  starting value and a fail level for every measure. I'll own it;
  follow-up 15 January 2027.

IT LEAD
- Worked: a 15-minute check-in with Vendor A every Monday, June to
  September. Problems were found the week they happened.
- Didn't work: we found the bad client email addresses only when the
  invitations bounced, which is where C3 came from.
- Change I propose: before any invitations go out, client services
  checks every client email in the practice system, and invitations
  start only when the check is signed off. Owner: Client services
  manager. Follow-up: 15 January 2027.

CLIENT SERVICES MANAGER
- Worked: inviting clients in batches of 50, in surname order. Support
  calls stayed under 15 a day the whole time (support log).
- Didn't work: nothing further.

TAX MANAGER
- Didn't work: when the bookkeeping clients were added (C1), nobody
  re-planned the automatic reminders. Only the first reminder was
  built; the second and third were not.
- Change I propose: keep everyone in the loop when the scope changes.
- On the measures: the timesheet code for chasing documents only
  started on 2 November, so there is no figure from before the portal.
- Also, one of the admin assistants kept forgetting to tag uploads by
  tax year, which made extra work.
```

### 6. The earlier changes (chosen at the review of the firm's last project)

```
Ref,Change,Owner,Follow-up date
E1,Every success measure has a fail level written down before work starts,Practice manager,2026-06-30
E2,A weekly check-in with the vendor during any system set-up,IT lead,2026-07-31
```

## The output

```
PROJECT LESSONS REVIEW: Client document portal, Phase 1, set-up and tax clients
DRAFT for the Practice manager. Changes are chosen by the project manager and delivery leads.

Review date: 12 November 2026. Planned 1 June 2026 to 25 September 2026; finished 16 October 2026.
Prepared from: the review brief; 7 deliverables; 3 changes; 4 measures; notes from the Practice manager, IT lead, Client services manager and Tax manager; 2 earlier changes.
Blameless: about practices and roles, never anyone's performance.

OUTCOME AGAINST THE AIMS
Aims: A1 Tax clients send their documents through the portal instead of by email. A2 Staff spend less time chasing missing documents. A3 Client files are complete before tax preparation starts.
Measures: 4. Met 2, short 1, missed 0, result due 1, not measured 0.
SHORT M1 Tax clients who have uploaded through the portal at least once (%) (A1): 58 against target 70, no fail level set, from 0. As of 6 November, Portal usage report.
MET M2 Client documents received by email in October (A1): 240 against target 300, fail level 600, from 1,850. As of 31 October, Email intake log.
RESULT DUE M3 Staff hours a week spent chasing missing documents (A2): Result due 11 December. Target 20, fail level 35, no starting value. Timesheets (new code from 2 November).
MET M4 Tax client portal accounts created (A1): 400 against target 400, fail level 350, from 0. As of 18 September, Portal admin report.
Aims with no measure: A3.
Verdict: PARTLY DELIVERED. Of the three measures with a result, two met their target and one fell short; M3's result is due on 11 December, and aim A3 has no measure.

SCOPE, SCHEDULE AND BUDGET
Scope: 6 deliverables in the original scope: 4 delivered, 1 partly delivered, 1 deferred, 0 dropped. 1 added.
  D4 Electronic signature for tax return authorisation forms: deferred. C2: Vendor A's signature module is not available in our region until January.
  D5 Portal accounts for 120 bookkeeping clients: added, delivered. C1: The partners asked for bookkeeping clients to join before year end.
  D7 Automatic reminders to clients with missing documents: partly delivered. No recorded change.
Schedule: planned finish 25 September, actual 16 October: 21 days later. Approved changes: +7 days (C1 +14, C2 -7). Recorded, not approved: +7 days (C3). Not traced to any recorded change: 7 days.
Budget: baseline $48,000; approved changes +$3,500 (C1 +$6,000, C2 -$2,500); approved budget $51,500; actual $55,300: $3,800 over the approved budget (7.4%). Recorded, not approved: $1,800 (C3). Not traced to any recorded change: $2,000.
Changes, in date order: 3
  C1, 8 July, scope: Add the 120 bookkeeping clients to phase 1. +14 days, +$6,000. Reason: The partners asked for bookkeeping clients to join before year end. Approved by: Managing partner.
  C2, 19 August, scope: Move electronic signature to phase 2. -7 days, -$2,500. Reason: Vendor A's signature module is not available in our region until January. Approved by: Managing partner.
  C3, 2 September, schedule: Extra data-cleaning days for client email addresses. +7 days, +$1,800. Reason: Duplicate and out-of-date client email addresses found when invitations bounced. Approved by: not on record.

THE SUCCESS MEASURES THEMSELVES
M1: Source: Portal usage report. Result by the review date: yes, 6 November. Shows its aim (A1): yes. Fail level: not set. Starting value: 0.
M2: Source: Email intake log. Result by the review date: yes, 31 October. Shows its aim (A1): yes. Fail level: yes, 600. Starting value: 1,850.
M3: Source: Timesheets (new code from 2 November). Result by the review date: no, due 11 December. Shows its aim (A2): yes. Fail level: yes, 35. Starting value: none recorded.
M4: Source: Portal admin report. Result by the review date: yes, 18 September. Shows its aim (A1): counts activity, not the aim; for the project manager to confirm. Fail level: yes, 350. Starting value: 0.
Aims with no measure: A3.
Said in the notes: Practice manager: M4 counted accounts created, which says nothing about whether clients use the portal, and M1 never got a fail level. Tax manager: the timesheet code for chasing documents started on 2 November, so there is no figure from before the portal.

WHAT WORKED, TO KEEP: 2
1. A 15-minute check-in with Vendor A every Monday, June to September; problems were found the week they happened. Evidence: IT lead's account. Raised by: IT lead.
2. Inviting clients in batches of 50, in surname order. Evidence: support calls stayed under 15 a day throughout (support log). Raised by: Client services manager.

PRACTICE CHANGES TO CHOOSE: 4
1. Seen in this project: C2 moved electronic signature (D4) to phase 2, -7 days and -$2,500, because Vendor A's signature module is not available in our region until January; it had been put in scope after the vendor's demo.
   Change: Before any feature goes into scope, the IT lead gets written confirmation from the vendor that it is available for the firm's account and region. As raised by the Practice manager.
   Owner: IT lead. Follow-up: not set.
   What would show it was used (proposed): a written vendor confirmation on file for each vendor feature in the next project's original scope.
   Chosen: yes [ ]  no [ ]  changed [ ]
2. Seen in this project: M1 had no fail level and M3 had no starting value.
   Change: Before work starts, the project manager records a starting value and a fail level for every measure. As raised by the Practice manager.
   Owner: Practice manager. Follow-up: 15 January 2027.
   What would show it was used (proposed): every row of the next project's measures export has a starting value and a fail level dated before its planned start.
   Extends earlier change E1, which was partly applied.
   Chosen: yes [ ]  no [ ]  changed [ ]
3. Seen in this project: C3 added 7 days and $1,800 of data cleaning after invitations bounced on duplicate and out-of-date client email addresses.
   Change: Before any invitations go out, client services checks every client email in the practice system, and invitations start only when the check is signed off. As raised by the IT lead.
   Owner: Client services manager. Follow-up: 15 January 2027.
   What would show it was used (proposed): a signed-off email check on file before the first invitation of the next client rollout.
   Chosen: yes [ ]  no [ ]  changed [ ]
4. Seen in this project: C1 added the 120 bookkeeping clients (D5), +14 days and +$6,000; the automatic reminders (D7) were then partly delivered, the second and third reminders not built.
   Change: When the sponsor approves a scope change, the project manager lists every open deliverable it affects, and each delivery lead confirms a new date or a smaller scope for theirs before work on the change begins. Proposed wording. Raised as: 'keep everyone in the loop when the scope changes' by the Tax manager.
   Owner: not named. Follow-up: not set.
   What would show it was used (proposed): each approved scope change in the next project's change log lists the deliverables it affects, with a confirmed date or scope for each.
   Chosen: yes [ ]  no [ ]  changed [ ]

EARLIER CHANGES FOLLOWED UP: 2
E1 Every success measure has a fail level written down before work starts (owner Practice manager, follow-up 30 June): Partly applied. M2, M3 and M4 have a fail level; M1 does not.
E2 A weekly check-in with the vendor during any system set-up (owner IT lead, follow-up 31 July): Applied. The IT lead's note records a check-in with Vendor A every Monday, June to September; the notes are silent on October, when the phase ran to 16 October.

REFERRED ELSEWHERE: 0
None.

QUESTIONS FOR THE PRACTICE MANAGER: 9
1. M3's result is due on 11 December. When will it be added to this review?
2. Aim A3, client files complete before tax preparation starts, has no measure. Should phase 2 have one?
3. D7 was partly delivered and no recorded change covers it; the Tax manager's note says the second and third reminders were not built after C1. Was the smaller scope agreed, and do the remaining reminders move to phase 2?
4. C3 has no approver on record. Was it approved, and by whom?
5. 7 days of the delay and $2,000 of the cost are not traced to any recorded change. What explains them?
6. M4 counts accounts created, not use. Should it stay a success measure for aim A1?
7. Practice change 1 has no follow-up date. When is it?
8. Practice change 4 has no owner and no follow-up date. Who owns it, and when is the follow-up?
9. A remark about one person was left out. It points to a step in the work, tagging uploads by tax year. Does the team want a practice change for that step?

Left out: 1 remark judging a person's work.
Prepared for the Practice manager's decision. Nothing has been sent, assigned or changed in any plan, register or record.
```

How the figures were reached. The phase finished 21 days after its planned date: 5 days from 25 to 30 September and 16 more to 16 October. Approved changes account for 7 of them (C1 +14, C2 -7), C3 for 7 more without an approver on record, and the last 7 are untraced. The approved budget is $48,000 + $6,000 - $2,500 = $51,500; the actual cost of $55,300 is $3,800 over it, which is 7.4% of $51,500; C3's $1,800 leaves $2,000 untraced. Of the three measures with a result, M2 (240 against a target of 300, where lower is better) and M4 (400 against 400) met their targets, and M1 (58 against 70) fell short with no fail level set, so the verdict is partly delivered. The tax manager's remark about one admin assistant was left out and only the step it points to was kept, as a question. The practice manager chooses the changes with the delivery leads, fills the missing owner and dates, answers the questions and then shares the review with the managing partner.
