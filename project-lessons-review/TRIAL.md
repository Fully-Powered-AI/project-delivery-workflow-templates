# Project lessons review: tried once on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-10

The inputs are the invented example published beside this record, in `public/example.md`: an invented 45-person accounting firm and its client document portal project. No client data was used. The assistant read the template and the six inputs (the review brief, deliverables list, change log, success measures, lessons notes and earlier changes), followed the instruction block and the output format, and produced the draft below without first seeing the published output. The two were compared afterwards. This is one run by one model; it shows that the instructions can be followed on this example, nothing more.

## What came out

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
Verdict: PARTLY DELIVERED. Of the three measures with a result, two are met and one is short; M3's result is due on 11 December, and aim A3 has no measure.

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
Said in the notes: Practice manager: M4 counted accounts created, which says nothing about whether clients use the portal; M1 never got a fail level. Tax manager: the timesheet code for chasing documents started on 2 November, so there is no figure from before the portal.

WHAT WORKED, TO KEEP: 2
1. A 15-minute check-in with Vendor A every Monday, June to September; problems were found the week they happened. Evidence: IT lead's account. Raised by: IT lead.
2. Inviting clients in batches of 50, in surname order. Evidence: support calls stayed under 15 a day the whole time (support log). Raised by: Client services manager.

PRACTICE CHANGES TO CHOOSE: 4
1. Seen in this project: C2 moved electronic signature (D4) to phase 2, -7 days and -$2,500, because Vendor A's signature module is not available in our region until January; it had been put in scope after the vendor's demo.
   Change: Before any feature goes into scope, the IT lead gets written confirmation from the vendor that it is available for the firm's account and region. As raised by the Practice manager.
   Owner: IT lead. Follow-up: not set.
   What would show it was used (proposed): a written vendor confirmation on file for each vendor feature in the next project's scope.
   Chosen: yes [ ]  no [ ]  changed [ ]
2. Seen in this project: M1 has no fail level and M3 has no starting value.
   Change: Before work starts, the project manager records a starting value and a fail level for every measure. As raised by the Practice manager.
   Owner: Practice manager. Follow-up: 15 January 2027.
   What would show it was used (proposed): every row of the next project's measures list has a starting value and a fail level recorded before the planned start.
   Extends earlier change E1, which was partly applied.
   Chosen: yes [ ]  no [ ]  changed [ ]
3. Seen in this project: C3 added 7 days and $1,800 of data cleaning after invitations bounced on duplicate and out-of-date client email addresses.
   Change: Before any invitations go out, client services checks every client email in the practice system, and invitations start only when the check is signed off. As raised by the IT lead.
   Owner: Client services manager. Follow-up: 15 January 2027.
   What would show it was used (proposed): a signed-off email check on file before the first invitation of the next client rollout.
   Chosen: yes [ ]  no [ ]  changed [ ]
4. Seen in this project: C1 added the 120 bookkeeping clients (D5), +14 days and +$6,000; the automatic reminders (D7) were then partly delivered, the second and third reminders not built.
   Change: When a scope change is recorded in the change log, the project manager re-plans every deliverable that depends on the changed scope and records the re-plan against the change reference. Proposed wording. Raised as: 'keep everyone in the loop when the scope changes' by the Tax manager.
   Owner: not named. Follow-up: not set.
   What would show it was used (proposed): each scope change in the next project's change log has a re-plan note listing the deliverables it affects.
   Chosen: yes [ ]  no [ ]  changed [ ]

EARLIER CHANGES FOLLOWED UP: 2
E1 Every success measure has a fail level written down before work starts (owner Practice manager, follow-up 30 June): Partly applied. M2, M3 and M4 have a fail level; M1 does not. The inputs do not show when the levels were written.
E2 A weekly check-in with the vendor during any system set-up (owner IT lead, follow-up 31 July): Applied. The IT lead's note records a check-in with Vendor A every Monday, June to September.

REFERRED ELSEWHERE: 0
None.

QUESTIONS FOR THE PRACTICE MANAGER: 10
1. D7 was partly delivered and no recorded change covers it; the Tax manager's note says the second and third reminders were not built after C1. Was the smaller scope agreed?
2. C3 has no approver on record. Was it approved, and by whom?
3. 7 days of the delay are not traced to any recorded change. What explains them?
4. $2,000 of the cost is not traced to any recorded change. What explains it?
5. M3's result is due on 11 December. When will it be added to this review?
6. Aim A3, client files complete before tax preparation starts, has no measure. Should the next phase have one?
7. M4 counts accounts created, not use. Should it stay a success measure for aim A1?
8. Practice change 1 has no follow-up date. When is it?
9. Practice change 4 has no owner and no follow-up date. Who owns it, and when is the follow-up?
10. A remark about one person was left out. It points to a step in the work, tagging uploads by tax year. Does the team want a practice change for that step?

Left out: 1 remark, judging a person's work.
Prepared for the Practice manager's decision. Nothing has been sent, assigned or changed in any plan, register or record.
```

## What was observed

- Every required part was produced. No stop condition was triggered: all headings matched, the brief was complete, no ID repeated, the work had ended, the currency and day count were the brief's.
- The figures match the published example: 21 days late (7 approved, 7 recorded but not approved, 7 untraced); approved budget $51,500; $3,800 over (7.4%); $1,800 recorded without approval and $2,000 untraced; M1 short with no fail level, M2 and M4 met, M3 result due 11 December; verdict PARTLY DELIVERED; A3 has no measure.
- Differences from the published example:
  - Ten questions against its nine. The template says one question for "days or cost not traced to any recorded change"; this run asked about the days and the cost separately, the example asked once.
  - The question order differs. This run followed the order of the list in step 11 of the instructions (scope, approver, untraced, result due, aim, activity, owner, remark). The example puts the result due and the aim with no measure first, which is the order of the output sections. The template says "in the order of the sections they come from", and the two orderings disagree.
  - The proposed wording for the tax manager's "keep everyone in the loop" differs. The example has the sponsor approving the change and each delivery lead confirming a new date or smaller scope; this run has the project manager re-planning every dependent deliverable and recording it against the change reference. Both name a step, a point in the project and a role.
  - Small wording differences in the "what would show it was used" lines, in the verdict sentence, and in the E1 line (this run adds that the inputs do not show when the fail levels were written). The example's question about A3 says "phase 2"; this run says "the next phase".
- Facts not in the inputs:
  - In this run's output, only the project manager as the role in the rewritten change 4. The notes do not say who should re-plan. The template forbids inventing an owner but requires the proposed wording to name a role, so the role is a guess from what a project manager does.
  - In the published example, the sponsor approving a scope change and each delivery lead confirming a new date are not in the inputs either. The example's note "5 days from 25 to 30 September and 16 more" is arithmetic, not a fact from the inputs.
- Where the instructions were ambiguous, and a choice had to be made:
  - The question order, and whether untraced days and untraced cost are one question or two (above).
  - A rewritten change must name a role, yet the owner must not be invented. The template does not say whether the role in the wording counts as naming an owner.
  - Whether a measure with no fail level (M1) or no starting value (M3) earns a question. Step 11 has no item for it, so none was asked, although the project manager's own change 2 covers the point.
  - E2: the notes record vendor check-ins from June to September, but the phase ran to 16 October and the notes are silent on October. This run marked it Applied, on the IT lead's account only. "Partly applied" would also be defensible.
  - E1 asks for fail levels "before work starts"; the inputs show only that levels exist, not when they were written. This run marked it Partly applied because of M1, and said the timing is not shown.
  - Whether "nothing to add" from the project manager counts as a thing that worked. It was treated as nothing raised.
- After this run the template was made explicit on the question order, the single question for untraced days and cost, the role in a proposed wording, the stop on a different currency or day count, the verdict for a measure never measured, and a few cases the instructions had left implicit; it was not run again, so the ambiguities above describe the template as it stood at the run.
- Nothing in the template told the assistant to stop on this example. The measures export had no fail level on M1 and no starting value on M3; blanks in those columns are handled by the template and are not a heading mismatch.
- Shortcomings: one run, one model, one example. The tests listed in the template ("proposed tests, none has been run") were not run. Only the happy path with a vague change, a remark about a person and an untraced remainder was exercised; the stop conditions, the incident referral and the decline cases were not.
