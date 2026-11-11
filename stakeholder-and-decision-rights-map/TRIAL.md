# Stakeholder and decision rights map: tried once on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-10

The inputs are the invented example in `public/example.md` (the brief, the stakeholder list, the decision list, the project manager's notes and the settings). No client data was used. The run was made by an assistant that had not written the template. It followed the instruction block and the output format in `member/template.md` on those inputs, and only afterwards compared its result with the published example output and the reviewer checklist.

## What came out

The draft below is the substantial part of what the run produced. Sections 1 to 3 are shortened here where the lines only repeat the inputs; sections 4 to 6 and the header are given in full.

```
STAKEHOLDER AND DECISION RIGHTS MAP: Handheld scanners in the warehouse, prepared 10 November 2026
DRAFT for the Project manager. Every decision right is a proposal until the Operations director and each accountable owner confirm it.

For: Project manager, with Operations director. Kickoff Monday 23 November 2026. Go-live Monday 8 February 2027. Phases: Plan ends Friday 11 December 2026; Build and test ends Friday 29 January 2027. Test window Monday 18 to Friday 22 January 2027.
Prepared from: stakeholder list (10 rows); decision list (6 decisions); project brief; the project manager's notes; settings as set (consult lead time and tell-after time at their defaults).
Stakeholders: 10. Decisions: 6. Decisions with exactly one accountable owner, on the list and in post: 3 of 6. Questions for the sponsor: 5. Questions for the project manager: 4.

1. EVERYONE AFFECTED
(ten lines, one per row, each repeating What changes, Controls and Told by as listed; the IT manager's line carries the note that the post is vacant from 4 January 2027 with no cover named, and the shift leads' line carries the note that in practice they decide whether a new routine sticks on the floor)
Coverage check:
  1. Sponsor and money: Operations director.
  2. Daily work or use of the result: Warehouse manager; Warehouse shift leads; Warehouse pickers and packers; Customer service team; (results) Operations director, Customer service lead.
  3. Owns a system, procedure or record: Warehouse manager; Customer service lead; IT manager.
  4. Approves the spending: Operations director (project budget); Finance controller (purchases above $10,000). Not covered: purchases of $10,000 or less.
  5. Signs off safety and security: none on the list (question 1 for the project manager). The IT manager controls the network and devices, but nothing says that includes sign-off.
  6. Supports it after go-live: Supplier A (repairs); IT manager (the warehouse system), post vacant from 4 January 2027. Not covered: who supports the system once that post is vacant (question 3 for the project manager).
  7. Outside the company: Supplier A; Trade customers.
  8. People's time borrowed: Warehouse manager (shift rotas); Customer service lead (staff rota).

2. INFLUENCE AND INTEREST
Placed by the rules unless marked "as listed".
Partner (high influence, high interest): Operations director; Warehouse manager; Warehouse shift leads (as listed); Customer service lead; IT manager
Brief (high influence, low interest): Finance controller; Supplier A
Involve (low influence, high interest): Warehouse pickers and packers; Customer service team
Notify (low influence, low interest): Trade customers
Placements to confirm: Warehouse shift leads: listed as high influence, high interest (Partner); the row gives Involve because it controls nothing and is accountable for no decision. Reason given: in practice they decide whether a new routine sticks on the floor. Confirm or change.

3. DECISION RIGHTS
D1 Approve the project scope and budget. Needed by Friday 27 November 2026. A: Operations director. R: Project manager. C: Finance controller; Warehouse manager; Customer service lead. I: IT manager.
D2 Choose the scanner model and order quantity. Needed by Friday 4 December 2026. A: IT manager; Warehouse manager. R: Project manager. C: Supplier A; Warehouse shift leads. I: Finance controller. FLAG, more than one accountable: two roles are listed. See section 4, question 1.
D3 Set the new order cut-off time for trade customers. Needed by Friday 11 December 2026. A: NONE. R: Customer service lead. C: Warehouse manager; Operations director; Transport planner. I: Customer service team; Trade customers. FLAG, no accountable owner, not on the stakeholder list: the Accountable cell is blank and the Transport planner has no row. See section 4, question 2, and section 6, question 2.
D4 Approve the new pick-and-pack procedure. Needed by Friday 15 January 2027. A: Warehouse manager. R: Warehouse shift leads. C: Warehouse pickers and packers. I: Customer service lead.
D5 Accept the scanners and warehouse system set-up as finished. Needed by Friday 22 January 2027. A: IT manager. R: Supplier A. C: Warehouse manager. I: Project manager. FLAG, accountable vacant: the IT manager's post is vacant from 4 January 2027. See section 4, question 3.
D6 Go live or postpone. Needed by Monday 1 February 2027. A: Operations director. R: Project manager. C: Warehouse manager; Customer service lead; IT manager. I: Warehouse pickers and packers; Customer service team; Trade customers; Finance controller. FLAG, consulted role vacant: the IT manager is consulted by Monday 25 January 2027 and the post is vacant from 4 January 2027. See section 6, question 3.
Letters tidied: none.

4. MISSING DECISION MAKERS: QUESTIONS FOR THE OPERATIONS DIRECTOR
1. D2 Choose the scanner model and order quantity, more than one accountable. The IT manager and the Warehouse manager are both listed; needed by Friday 4 December 2026. Which one has the final word?
2. D3 Set the new order cut-off time for trade customers, no accountable owner. The Customer service lead prepares it; the Warehouse manager, Operations director and Transport planner are consulted; needed by Friday 11 December 2026. Who has the final word?
3. D5 Accept the scanners and warehouse system set-up as finished, accountable vacant. The IT manager is listed; needed by Friday 22 January 2027; the post is vacant from 4 January 2027 with no cover named. Who is accountable on that date?
Standard decisions: scope and budget D1; spending beyond the budget not on the list; scope change after approval not on the list; go-live date D6 (go live or postpone); accepting the finished work D5 (scanners and warehouse system set-up only).
4. Not on the list: approve spending beyond the approved budget. Who decides it?
5. Not on the list: change the scope after it is approved. Who decides it?

5. COMMUNICATION PLAN
Operations director (Partner). Told by: project manager. Concerns raised: none recorded. Touchpoints: Tuesday project meeting, weekly, Tuesday 24 November 2026 to Tuesday 2 February 2027, none on Tuesday 29 December 2026 (closed). Decisions: accountable for D1 and D6; consulted on D3 by Friday 4 December 2026.
Warehouse manager (Partner). Told by: project manager. Concerns raised: none recorded. Touchpoints: as above. Decisions: accountable for D2 (jointly listed) and D4; consulted on D1 by Friday 20 November 2026, D3 by Friday 4 December 2026, D5 by Friday 15 January 2027, D6 by Monday 25 January 2027.
Warehouse shift leads (Partner, as listed). Told by: Warehouse manager. Concerns raised: none recorded. Touchpoints: as above. Decisions: responsible for D4; consulted on D2 by Friday 27 November 2026.
Customer service lead (Partner). Told by: project manager. Concerns raised: none recorded. Touchpoints: as above. Decisions: responsible for D3; consulted on D1 by Friday 20 November 2026 and D6 by Monday 25 January 2027; told of D4 by Tuesday 19 January 2027.
IT manager (Partner). Told by: project manager. Concerns raised: none recorded. Touchpoints: Tuesday project meeting, Tuesday 24 November to Tuesday 22 December 2026; vacant from 4 January 2027, no touchpoints after. Decisions: accountable for D2 (jointly listed) and D5 (vacant on its date); consulted on D6 by Monday 25 January 2027 (vacant on that date); told of D1 by Tuesday 1 December 2026.
Finance controller (Brief). Told by: project manager. Concerns raised: none recorded. Touchpoints: written note, email, Friday 11 December 2026 and Friday 29 January 2027. Decisions: consulted on D1 by Friday 20 November 2026; told of D2 by Tuesday 8 December 2026 and D6 by Wednesday 3 February 2027.
Supplier A (Brief; outside). Told by: Project manager. Concerns raised: none recorded. Touchpoints: written note, email, Friday 11 December 2026 and Friday 29 January 2027. Decisions: responsible for D5; consulted on D2 by Friday 27 November 2026.
Warehouse pickers and packers (Involve). Told by: Warehouse shift leads. Concerns raised: none recorded. Touchpoints: question-and-answer session, team huddle, by Friday 27 November 2026; hands-on session, team huddle, Monday 18 to Friday 22 January 2027; written update, noticeboard, Friday 11 December 2026 and Friday 29 January 2027; go-live notice, noticeboard, Wednesday 3 February 2027. Decisions: consulted on D4 by Friday 8 January 2027; told of D6 by Wednesday 3 February 2027.
Customer service team (Involve). Told by: Customer service lead. Concerns raised: at their team meeting on Tuesday 3 November 2026, that a 2 pm cut-off will bring complaints from trade customers who order late in the day. Touchpoints: as for the pickers and packers. Decisions: told of D3 by Tuesday 15 December 2026 and D6 by Wednesday 3 February 2027.
Trade customers (Notify; outside). Told by: messenger not named (section 6, question 4). Concerns raised: none recorded. Touchpoints: go-live notice, email, Wednesday 3 February 2027. Decisions: told of D3 by Tuesday 15 December 2026 and D6 by Wednesday 3 February 2027.

6. QUESTIONS FOR THE PROJECT MANAGER
1. Nobody on the list signs off safety and security for the scanners or the new way of picking. Who does, and should they have a row?
2. The Transport planner is consulted on D3 but has no row. Please supply one.
3. The IT manager's post is vacant from 4 January 2027 with no cover named. The role is consulted on D6 (by Monday 25 January 2027) and supports the warehouse system after go-live. Who takes its place from that date?
4. Nobody is named to tell the trade customers. Who tells them?
Left out: 1 remark about an individual, not repeated.

Next review of this map: Friday 11 December 2026, when Plan ends.
Decision rights confirmed with the Operations director: [ ]  Date: [ ]
Draft for the Project manager. Nothing has been sent, booked, assigned or changed in any record.
```

## What was observed

Everything required was produced. Every section was filled, nothing needed the run to stop, and the counts (10 stakeholders, 6 decisions, 3 of 6 decisions with one accountable owner in post, 5 questions for the sponsor, 4 for the project manager) agree with the body. Nothing was sent, booked or assigned. The remark about the finance controller in the notes was left out and counted, and is not repeated here. No password or login code appeared in the inputs.

Compared with the published example output, the run matched on placements, flags, questions, dates and the communication plan, line for line apart from wording. The differences were these:

- Coverage question 5 (safety and security). The run wrote "none on the list" and noted that the IT manager owns the network and devices. The example credits the IT manager for security and says only safety is not covered. The template does not say whether owning the network counts as signing off security, so both readings fit.
- Coverage question 4. The run added that purchases of $10,000 or less are not covered. The example does not.
- Coverage question 6. The run added that nobody is named to support the system once the IT manager's post is vacant. The example points to its question 3 instead.
- Coverage question 2. The run also listed the two rows whose results change.
- The example gives each of the ten stakeholder lines in full; the run shortened the plan lines for the second to fourth Partner rows and for the second Involve row to "as above" in the version recorded here only.
- The standard-decision check. The run added the words "go live or postpone" and "scanners and warehouse system set-up only" after D6 and D5, to show what each does and does not cover. The example just names the IDs.

No fact appears in either output that is not in the inputs. Every date matched on recount, and every weekday was right.

Where the template was ambiguous, and the run had to choose:

1. **Notify and the go-live notice.** The Notify default reads "a go-live notice 3 working days before go-live for every row". It can mean every Notify row or every row on the map. The run took it as every Notify row, because Partner and Brief have no such notice, and the example agrees.
2. **Settings "default".** The brief header offers "default settings" or "settings as set". Here the meeting day and channels were set but the two lead times said "default". The run wrote "settings as set" with a note; the example writes "settings as set". The template does not say which applies to a mix.
3. **Channel for each kind of touchpoint.** The settings give one channel per group (for Involve, "a team huddle and the noticeboard") with no rule for which kind of touchpoint uses which. The run used the huddle for sessions and the noticeboard for written updates.
4. **The hands-on session.** The template says "in the test window" and gives no date, so the line carries the whole window.
5. **What counts as "covering" a standard decision.** D6 "Go live or postpone" is taken as covering "set or move the go-live date", and D5 as covering "accept the finished work", though D5 speaks only of the scanners and the system set-up. The template gives no test for covering.
6. **Partly answered coverage questions.** Step 2 says to write what the list does not cover, and that an unanswered question becomes a question for the project manager. It does not say whether a partial answer also does. The run made a question only for question 5 and folded question 6 into the vacancy question.
7. **Consult dates before kickoff.** D1's consult-by date, Friday 20 November 2026, falls three days before kickoff and four before the first weekly meeting. The template allows it and does not say how to bring it to the project manager's attention.
8. **Told by on one-person rows.** Section 1 prints "blank" where the list is blank, while section 5 says "project manager". This is correct by the rules but reads as an inconsistency.
9. **Controls against the decision chart.** The finance controller "approves the scanner purchase" but is only informed of the purchase decision (D2). The template does not check what a row controls against what it is accountable for, so this passed unflagged. The sponsor may want to look at it.

Shortcomings of this single run. It tested one invented example, by one assistant, in one product. It did not test the stop conditions (an unmatched heading, no brief, a request to send a message), the acceptance tests in the template, or an input with a vacancy before a consult date. Nothing here shows how it behaves with real lists, longer decision lists or other AI products.

## After the run

Following a second independent review, the template was edited and not run again; the record above is of the earlier wording and is unchanged. The edit settled the points this run raised as ambiguities 1, 4, 5, 6 and 8: the go-live notice for Notify goes to every Notify row; the hands-on session is shown as the whole test window; a listed decision covers a standard one only if it decides the same thing for the whole project; safety and security are answered separately in coverage question 5, so a missing safety row is a question for the project manager, as the published example shows; and section 1 prints "Told by" as listed while section 5 gives the messenger used. The run's own reading of coverage question 5 ("none on the list") is not what the template now asks for.

The published example's standard-decision line was then changed to match that rule and now reads "accepting the finished work D5 (scanners and system set-up only)", so the difference noted above for D5 no longer shows; D6 is still named by its ID alone.
