# Scope change impact review: tried once on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (`claude-sonnet-5-5`). It did not write the template.
- **Date:** 2026-11-10

The inputs were the invented example's seven inputs (settings, baseline facts, baseline deliverables, working list, change log, request notes, estimates), exactly as published in `public/example.md`. No client data was used. The run read the template and those inputs only, followed the instructions block and the output format, and produced the review below before the example's own output was read. The two were compared afterwards.

## What came out

```
SCOPE CHANGE IMPACT REVIEW: Client portal, as of Tuesday 10 November 2026
DRAFT for the project manager. The operations director accepts or declines each change.

For: operations director. Baseline approved Monday 14 September 2026 by the operations director. Approvers of changes: operations director.
Compared: 6 baseline deliverables; 11 rows in the working list; 2 change-log rows; request notes: meeting notes of 22 October and two emails; estimates for 3 of 4 pending changes.

POSITION
Baseline: 6 deliverables, 55 days, $39,750, end date Friday 4 December 2026.
Approved changes: 1 (CR-01): +7 days, +$5,750. Now 62 days, $45,500, end date Friday 11 December 2026.
Pending changes: 4: +23 days, +$19,150 for those estimated; not estimated: A5. If all were accepted: 85 days, $64,650, plus A5, not estimated. End dates are shown for each change alone and are not added together.

WORK STARTED WITHOUT APPROVAL: 2
D5 Migration of 55 help articles. Status: In progress. Due in the working plan 20 November.
A2 Document request checklist for each client. Status: In progress. Due in the working plan 25 November.

DECISIONS FOR THE OPERATIONS DIRECTOR: 4
1. Accept or decline D5 Migration of 55 help articles, changed from the baseline "Migration of 40 help articles"?
   Asked for by: the content lead, for the tax and advisory teams, 4 November (email).
   Status: In progress, work started without approval.
   Effect: 3 days; $1,950 (3 days at $650, no other cost); end date Friday 11 December 2026 if accepted alone (no change), per the portal lead.
   Assumptions: 15 more articles at the same pace as the first 40; fits before launch.
   In the working plan for: 20 November.
2. Accept or decline A2 Document request checklist for each client?
   Asked for by: the tax manager, 22 October (meeting notes). Agreed in the notes by the portal lead, who is not an approver; that is not an approval.
   Status: In progress, work started without approval.
   Effect: 9 days; $8,250 (9 days at $650, plus $2,400 other); end date Friday 18 December 2026 if accepted alone (+5 working days), per the portal lead.
   Assumptions: Needs the portal's reminder add-on, $2,400 for a year.
   In the working plan for: 25 November.
3. Accept or decline A5 Saved favourite documents?
   Asked for by: not found.
   Status: Not started.
   Effect: not estimated.
   Assumptions: none given.
   In the working plan for: 27 November.
4. Accept or decline A3 Card payment of invoices?
   Asked for by: the finance director, 2 November (email).
   Status: Not started.
   Effect: 11 days; $8,950 (11 days at $650, plus $1,800 other); end date Tuesday 5 January 2027 if accepted alone (+10 working days, skipping closed days), per the portal lead.
   Assumptions: Card payment provider's set-up fee, $1,800; finance opens the provider account.
   Appears to match the baseline exclusion "Online payment of invoices by card".
   In the working plan for: 30 November.

COMPARISON WITH THE BASELINE
Unchanged: 4 of 6 baseline deliverables (D1, D2, D3, D4).
Approved additions and changes: A1 Appointment booking with advisers, CR-01, operations director, 16 October.
Not approved: D5 (changed wording), no change-log entry; A2, no change-log entry; A3, no change-log entry; A5, no change-log entry.
Declined but still in the working plan: A4 Pages in Spanish, CR-02, operations director, 30 October.
Dates moved: D6 Launch and client invitation emails, from 4 December to 11 December; not later than the current end date.
Baseline deliverables not in the working list: none.
Approved changes not in the working list: none.
Requests in the notes not in the working list: a printable summary of each client's open requests, the audit partner, 22 October (meeting notes).

FOR THE PROJECT MANAGER ONLY. Remove before sharing.
Questions: 6
1. D5 Migration of 55 help articles is in progress without an approved change. Should the work continue until the operations director decides?
2. A2 Document request checklist for each client is in progress without an approved change, and the portal lead agreed to it in the 22 October meeting. Should the work continue until the operations director decides?
3. A4 Pages in Spanish was declined on 30 October (CR-02) but is still in the working plan. Should it be removed, or does it go back to the operations director?
4. A5 Saved favourite documents has no request in the notes and no estimate. Who asked for it, and can the portal lead estimate it before the decision?
5. A3 Card payment of invoices appears to match the baseline exclusion "Online payment of invoices by card". Is it the same work?
6. The audit partner asked on 22 October for a printable summary of each client's open requests; it is not in the working list or the change log. Is it to go to the operations director as a change?
Prepared for the project manager. Nothing has been accepted, declined, added to or removed from the plan, estimated, or sent.
```

The sums were recomputed: the baseline's 6 + 12 + 18 + 5 + 8 + 6 is 55, matching the stated total, so the run went ahead. CR-01 is 7 days at $650 plus $1,200, which is $5,750. A3's ten working days from Friday 11 December run 14 to 18 December, 21 to 23 December, then 4 and 5 January, because 24 December to 1 January is closed.

## What was observed

- Every part of the output format was produced, in the stated order, and nothing was stopped for: all headings matched, the baseline added up, no `Ref` repeated, and nothing asked for a password.
- Nothing in the inputs triggered a refusal, so the refusal rules were not exercised by this run.
- The output matches the published example in every figure, date, ordering, classification and count. It differs only in small wording: role names in lower case, "(email)" and "(meeting notes)" without naming who received them, and the wording of the six questions. The template does not fix the wording of a question, so those differences are expected.
- Facts not in the inputs:
  - In my output, none. One phrase is an inference from the inputs, "for the tax and advisory teams" on D5, taken from the content lead's email.
  - In the example's output, one small addition. Its sixth question offers "back to the audit partner as out of scope", and nothing in the inputs says the audit partner's request is out of scope. Its other facts are in the inputs.
- Places the instructions left me to guess:
  - **The amount in the Position lines.** The format says "[amount]" for the baseline and the current position. The baseline facts give a budget of $39,750 that includes a $4,000 licence on top of the day-rate work. I used the budget and added the approved cost to it. The template does not say whether the amount is the budget or the day-rate cost, and the two give different numbers ($35,750 against $39,750).
  - **How to order "Work started without approval".** The template orders the decisions and the questions but not this list. I used due date, as the decisions do.
  - **D6's date moved.** D6 moved from 4 to 11 December without a change-log entry of its own. The rules only ask a question when a date moves later than the current end date, and 11 December equals the current end date, so no question was raised. Whether a date move needs its own approval is not covered.
  - **D5.** The content lead wrote that they had "changed the migration". The template asks whether a non-approver agreed in the notes. It is not clear whether the person who made the change counts as having agreed, so I did not add an "Agreed in the notes" line for D5.
  - **A4 and the exclusion check.** Pages in other languages is also on the exclusions list, but A4 is declined, so step 7 does not apply. The template is silent on whether to mention it.
  - **"Approved" in step 4** reads as "an approved change names its Ref", while step 2 requires an approver's decision. They agree in this example, but the two steps define approval differently.
  - **The question wording and the "Asked for by" wording for a person who made a change themselves** are left to the assistant.
- The acceptance tests in the template are marked "None has been run". This run covered only the worked example; it did not run any of the fourteen tests, so it says nothing about the stop conditions or the refusals.
- This is one run by one model on one invented example. It shows the instructions can be followed to the published result. It is not a test for a client and says nothing about real project data.

## Edits made after this run

These edits were made to the template and the example after the run above, on 10 November 2026, in answer to an earlier review. They have not been run again, and nothing above was changed to match them.

- The template now says the baseline amount in the position is the budget in the baseline facts and the current amount is that budget plus approved cost.
- The list of work started without approval now follows the same order as the decisions.
- A date move is now stated to need no change-log entry of its own.
- The "Agreed in the notes" line is now stated to apply only to a person other than the requester.
- A declined change is now stated not to be checked against the exclusions.
- The example's sixth question now reads "Does it go to the Operations director as a change?", dropping the offer of "back to the audit partner as out of scope" noted above.
- A second round of small edits followed an independent review, also not run again. The instruction block now carries the date and amount formatting rule, the "not costed: day rate not set" wording, the handling of a change-log row whose `Ref` is in neither list, and the wording "skipping closed days"; approved effort is now stated as the sum of the rows that stand; step 4 now says an approved change is as defined in step 2; and the exception allowing a recommendation on written request was dropped. None of these changes the example's inputs or output.
