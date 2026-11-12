# Project scope baseline: a trial on the invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-10

The inputs were the invented example in `public/example.md` (the settings, the approved brief, the discovery notes and constraints, and the sponsor's expectations). No client data was used. The run followed the instruction block and the output format in the workflow template exactly, in one pass, with no help from a person. The template was written by someone else.

One caveat on the method. The run was meant to be blind to the example's output until it had finished. A first read of the example file went too far and showed the output's first deliverables (D1 and D2) before the run began. The rest of the output was not read until the run was done. That may have nudged the wording of D1 and D2, so treat the match on those two as less independent than the rest.

## What came out

```
SCOPE BASELINE (DRAFT): Client document portal

For: Managing partner (sponsor) and Operations manager (project manager). Prepared Thursday 12 November 2026 from: the project brief (approved Monday 2 November 2026), discovery notes (9 November 2026), constraints (10 November 2026), the sponsor's expectations (10 November 2026), no working deliverable list supplied.
Status: draft, not baselined. Open questions: 10, of which 9 block baselining.
Purpose, from the brief: "Clients send documents by email and ask us where their work stands. Staff spend too much time chasing documents."

Deliverables: 4
D1 A client portal on Vendor A's platform. Source: brief, "What the project delivers", item 1.
   What it is: a portal where each client can upload documents and see a status for each of their open engagements.
   Accepted when: (1) a client can upload documents in the portal; (2) a client can see a status for each of their open engagements; (3) the brief's "clients find it easy to use" has no test yet (question 6).
   Accepted by: not stated (question 5).
D2 The open-engagement folders (140 today) moved from the shared drive into the portal. Source: brief, item 2.
   What it is: the open-engagement folders moved from the shared drive into the portal.
   Accepted when: (1) every open-engagement folder is in the portal, the count being "140 today" (question 8); (2) whether the folders stay on the shared drive is unsettled (question 1).
   Accepted by: not stated (question 5).
D3 A one-page guide for clients on how to use the portal. Source: brief, item 3.
   What it is: a one-page guide for clients on how to use the portal.
   Accepted when: (1) the guide is one page. No other check is stated in any source.
   Accepted by: not stated (question 5).
D4 Training for the 35 staff who work with clients. Source: brief, item 4.
   What it is: training for the 35 staff who work with clients.
   Accepted when: (1) the 35 staff who work with clients are trained; "trained" has no test yet (question 9); (2) no session falls on Monday 18 to Friday 22 January 2027 (K4).
   Accepted by: not stated (question 5).

Excluded: 2
X1 Integration with the billing system. Source: brief, "Not in this project".
X2 A mobile app. Source: brief, "Not in this project".

Constraints: 5
K1 Date: go-live on Monday 1 March 2027. Source: brief, "Targets".
K2 Budget: total $48,000, which includes the first year of Vendor A's fees, quoted at $18,000. Source: brief, "Targets"; constraints (10 November). Arithmetic: $48,000 - $18,000 = $30,000 left for everything other than those fees. Check: $30,000 + $18,000 = $48,000.
K3 People: the operations manager is away from Monday 21 December 2026 to Monday 4 January 2027. Source: constraints (10 November).
K4 People/rule: no staff training can be held from Monday 18 to Friday 22 January 2027 (firm retreat). Source: constraints (10 November).
K5 Platform: Vendor A's standard plan includes 50 staff seats. Source: discovery notes (9 November). (question 10)

Open questions for the sponsor: 10
1. Blocking, conflict. The brief, item 2, says the open-engagement folders are "moved from the shared drive into the portal". The sponsor said on 10 November: "Leave the shared drive alone for now." What is to be done about the shared-drive folders, given both statements? Affects: D2.
2. Blocking, implied deliverable. Discovery notes (9 November): "Team leads want clients to be able to send messages to staff inside the portal." The brief does not name it. Is client messaging inside the portal a deliverable or excluded? Affects: D1.
3. Blocking, implied deliverable. Discovery notes (9 November): closed engagements from the last three years, "about 600 folders", "must stay searchable by staff. Nobody has decided where they will live." The brief names no such work. Is making them searchable a deliverable or excluded? (If a deliverable, the "about 600" count would need a fixing date or rule.) Affects: D1, D2.
4. Blocking, implied deliverable. The sponsor said on 10 November: "Clients should be able to pay their invoices there too." The brief names no payment feature, and excludes "integration with the billing system" (X1). Is paying invoices in the portal a deliverable or excluded? Affects: D1, X1.
5. Blocking, no acceptor. No source says who accepts D1, D2, D3 or D4. Who accepts each? Affects: D1, D2, D3, D4.
6. Blocking, vague criterion. Brief, "Success": "clients find it easy to use". There is no test for "easy to use". What would be accepted instead? Affects: D1.
7. Blocking, vague criterion. Brief, "Success": "document-chasing emails drop significantly". There is no test for "significantly" and no starting figure or period. What would be accepted instead, and is it a criterion for the project or a result to look for after go-live? Affects: D1.
8. Blocking, unfixed figure. Brief, item 2: "140 today". On what date, or by what rule, is the number of open-engagement folders fixed? Affects: D2.
9. Blocking, vague criterion. Brief, item 4: "Training for the 35 staff who work with clients". No source says what makes a person trained (attendance, a test, a number of sessions). What would be accepted? Affects: D4.
10. Not blocking, constraint check. Discovery notes: Vendor A's standard plan includes "50 staff seats"; the firm has "60 staff". No source says how many people need a seat, and the brief says 35 staff work with clients. How many seats are needed? Affects: K5, D1.

Set aside, not scope: 2
- "Send me a one-paragraph progress note every Friday." Source: sponsor (10 November). A reporting request, not a deliverable of this project.
- "document-chasing emails drop significantly" (the second half of the brief's "Success" line). Source: brief, "Success". A result to look for after go-live, not something handed over (see question 7).

Sign-off (to be completed by people, after the questions are answered)
Operations manager: ____________  Date: ________
Managing partner: ____________  Date: ________

Internal working document for Client document portal, not a client statement of work or a contract. Nothing has been sent, filed, changed or baselined.
```

## What was observed

Every part of the output format was produced: the header and status line, the purpose, deliverables with criteria and acceptors, exclusions, constraints, questions, the set-aside list, blank sign-off lines and the closing line. The counts were checked at the end (4 deliverables, 2 exclusions, 5 constraints, 10 questions of which 9 block, 2 set-aside items) and every item in the brief and the other inputs was placed. Nothing in the inputs told the run to stop, and no stop condition was met. The run asked for nothing, decided nothing, and left the sign-off blank.

Where it matched the published example:

- The same four deliverables, the same two exclusions from the brief, and the same $30,000 calculation ($48,000 - $18,000), shown with its working and checked.
- A question for each of messaging, the closed folders and invoice payment; none became a deliverable or an exclusion.
- One question for the missing acceptors, a vague-criterion question for "easy to use", an unfixed-figure question for "140 today", and a question on what counts as trained.
- The Friday progress note and the "drop significantly" line were set aside.

Where it differed from the published example:

- Questions: this run had 10 with 9 blocking; the example has 10 with 8 blocking.
- Invoice payment: this run made it a blocking implied-deliverable question (the brief names no payment feature, and X1 only excludes billing integration). The example calls it a conflict.
- "Leave the shared drive alone for now": this run used it only in the conflict question with D2 and did not list it as an exclusion. The example lists it as an exclusion (X3), marks it "Not in the brief" and adds a not-blocking question on it. This run would have been listing an exclusion that contradicts D2.
- "document-chasing emails drop significantly": this run also asked a blocking vague-criterion question about it. The example only sets it aside.
- Constraints: this run had five (budget and vendor fees together in one line); the example has six.
- D3: this run gave one check (one page); the example adds "it covers how to use the portal".
- D4: this run linked the training blackout in January to the deliverable's criteria; the example does not.
- Sign-off lines: this run used the roles from the settings (Operations manager, Managing partner); the example prints "Project manager" and "Sponsor".
- Seats: this run asked how many seats are needed and did not state that 35 fit within 50 and 60 would not; the example states both.

Facts not in the inputs:

- In this run's output: none found on a second read. Weekdays for the dates were taken from the inputs or checked against the calendar.
- In the example's output: "Moved folders leave the shared drive; copied folders do not" and the question "moved or copied?" go beyond the inputs and offer an option, which the template says not to do unless a source does. "If it is a deliverable, X1 has to be reworded" is also a recommendation no source gave. "Who decides which engagements are open" and "who runs the test" are questions the inputs do not raise, which is allowed. X3 reads "Any change to the shared drive", wider than the sponsor's "for now".

Ambiguities in the template that the run had to settle by guessing:

1. Invoice payment: conflict or implied deliverable. Step 7 says a conflict is an exclusion and a deliverable that cannot both stand; payment is not a deliverable, and the exclusion is billing-system integration, which is not the same thing. The run chose implied deliverable.
2. A sponsor remark that cuts against a deliverable (the shared drive). Step 5 says an exclusion is whatever a source explicitly puts out of scope; step 7 says conflicts are never resolved. Listing it as an exclusion would put an exclusion beside a deliverable that contradicts it. The template does not say which step wins.
3. A vague word in a success line that belongs to no deliverable ("drop significantly"). Step 8 says set it aside; the reviewer checklist (item 3) says every vague word has a question. The run did both.
4. Whether the word "training" is vague. The list of untestable words is not exhaustive, so the run raised it. A different reader might not.
5. What to write under "Accepted when" for a deliverable where no source gives a check (D3, D4). The format covers a vague word or a missing test with a question number, but not a deliverable with nothing at all. The run wrote "no other check is stated".
6. The constraint-check question needs two limits that "cannot both hold". Nothing in the inputs says all 60 staff need a seat, so the limits do not clearly clash. The run asked anyway, as not blocking.
7. "About 600" closed folders is an unfixed figure, but step 4 attaches the unfixed-figure rule to deliverables' criteria, and these folders are not a deliverable. The run folded the point into the implied-deliverable question rather than adding another.
8. Step 1 says to count the items in the brief, but the brief mixes four numbered deliverables with "Why", "Not in this project", "Targets" and "Success" lines. What counts as an item is not defined.
9. The "For" line says to write "role not stated" for a missing role, and the closing line and sign-off use the roles; the example's sign-off uses the generic labels instead. The format is clear enough, but the two disagree.
10. A question must hold "one question to the sponsor", yet several natural questions here have two parts (who fixes the date, and what the date is). The run kept most to one, and split none.

The template's own instructions were clear on the stop conditions, the arithmetic, the ordering of questions and the sign-off; none of them was tested hard by this example. The record refers to the template's procedure steps by number and paraphrases some of its rules; no passage of the template was copied into it beyond the output itself.

## Edits made after this run

These edits were made to the template and the example after the run above, on 10 November 2026, in answer to an independent review. The comparison with the published example above describes the example as it stood at the time of the run. Several statements in it are no longer true of the example as published now (for instance, that it calls invoice payment a conflict, that its sign-off prints "Project manager" and "Sponsor", and the wording quoted from its questions and from X3). Nothing above was changed to match, and the edits have not been run again. Two small further edits followed a second review: the template now says a question with two parts is split into two numbered questions, which the run above did not have; and the example's D3 now reads "No other check is stated in any source" after its one-page check.

In the template:

- A remark from outside the brief that cuts against a deliverable is now listed as an exclusion marked "Not in the brief" and also raised as a conflict.
- A request near an exclusion but not the same thing (invoice payment beside the exclusion of billing-system integration) is now an implied-deliverable question that quotes the exclusion, not a conflict.
- A vague word in a result set aside as not scope is now quoted there with a note that it states no test, and gets no question unless it bears on a deliverable's acceptance.
- A deliverable with no stated check now reads "No check is stated in any source."
- The constraint check now covers a limit that sits beside a count from another source.
- Later clarifications: a deliverable described only as a state with no test ("trained", "delivered") gets a vague-criterion question; an unfixed figure inside an implied-deliverable question is quoted there and gets no separate question; the count of items in the brief is defined; the pasted instructions now carry the stops for a request outside the project and for notes on a named person's performance or pay, and the note that a deliverable merely named with a vague word is not vague. The third acceptance test now says the sponsor expects the very thing the brief excludes.

In the example:

- Invoice payment is now a blocking implied-deliverable question, not a conflict.
- The options and recommendations were removed from the first two questions.
- X3 now reads in the sponsor's words ("The shared drive left alone for now").
- The sign-off lines now use the roles from the settings.
- Questions 6, 7 and 10 now each ask one question; constraint types are now budget, platform, date and people from the template's list; the set-aside quotation now matches the brief's wording.
