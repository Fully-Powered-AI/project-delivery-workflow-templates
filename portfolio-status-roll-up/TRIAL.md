# Project portfolio status roll-up: trial on the invented example

- **Product:** Claude, run in Claude Code

**Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5). **Date:** 2026-11-12.

The inputs are the invented example in `public/example.md` (the settings, the register of five projects, four status reports, the last roll-up and the decision notes). No client data was used. The run followed the instruction block in `member/template.md` and its output format. The model that ran it did not write the template.

One thing to know before reading the result: this was meant to be a blind run, with the example's output read only afterwards. It was not fully blind. While reading the inputs, the model's file display ran on past them and showed the example's output before the run was made. The run below was done after that, so it may lean toward the published example. It still followed the template's steps, and the differences found are real, but a clean trial would use a reader who has not seen the output.

## What came out

The full draft, as the template's output format asks:

```
PORTFOLIO STATUS ROLL-UP: Internal projects, 26 October to 6 November 2026
DRAFT for the Head of operations' confirmation. Not for sending until confirmed.

For: Leadership team, meeting Tuesday 10 November 2026. Report date: 9 November 2026. Last roll-up: 26 October 2026.
Prepared from: the project register (5 projects); reports from 4 of 5 projects, none from: P5; the last roll-up of 26 October 2026; the decision notes.
Each status is as its lead stated it. This roll-up sets none of its own.

AT A GLANCE
5 projects: 1 red, 1 amber, 1 green, 1 not stated as a colour, 1 not reported.
Changed since the last roll-up: P2 from AMBER to GREEN; P3 from GREEN to not stated as a colour; P4 from GREEN to RED; P5 from GREEN to not reported.
Decisions asked of leadership: 3, earliest needed by 6 November, 1 past the date needed. Contradictions between reports: 2. Other gaps: 4.

DECISIONS ASKED OF LEADERSHIP: 3, earliest date needed first
D2 (P1, asked by IT manager, carried from the roll-up of 26 October). Should sales staff stop editing customer records until go-live (a data freeze), and from when? Needed by 6 November, past the date needed. Options given: freeze from 16 November; freeze from 7 December. Recommendation: IT manager: freeze from 16 November. What moves: not stated.
D3 (P1, asked by IT manager). Approve six extra days of the ERP supplier's consultant at $1,200 a day ($7,200)? Needed by 13 November. Options given: approve the days; go without them. Recommendation: IT manager: approve the days. What moves: with the days the cleansing finishes by 4 December and go-live holds at 1 February 2027; without them it finishes on 18 December and go-live moves to 1 March 2027.
D4 (P4, asked by Logistics manager). Rent temporary storage for December at $4,500, or hold the second line's incoming parts at their supplier until January? Needed by 16 November. Options given: rent the storage; hold the parts at the supplier until January. Recommendation: Logistics manager: rent the storage. What moves: without one or the other, parts arriving from 30 November have nowhere to go.
Answered since the last roll-up: D1, card and account credit for the dealer portal, by the leadership team, 30 October.

PROJECTS
P4 Warehouse racking and move. Lead: Logistics manager. Status: RED (last roll-up: GREEN).
  Reason, as stated: the racking supplier moved installation from 16 to 30 November because its steel delivery is late.
  Moved: floor marking finished; fire inspection of the new bay passed 2 November.
  End: planned 27 November; lead's forecast 11 December (the move out of the old bay finishes then).
P1 New ERP system. Lead: IT manager. Status: AMBER (last roll-up: AMBER).
  Reason, as stated: customer and price data cleansing is two weeks behind plan because the ERP supplier moved its consultant to another client for a week.
  Moved: chart of accounts mapped and signed off 28 October; test system live 3 November.
  End: planned 1 February 2027; lead's forecast 1 February 2027, if the cleansing finishes by 4 December; 1 March 2027, without the extra days.
P2 Second assembly line. Lead: Plant engineer. Status: GREEN (last roll-up: AMBER).
  Reason, as stated: no reason given.
  Moved: four machines arrived 30 October; delivery inspection passed 2 November.
  End: planned 15 January 2027; lead's forecast 15 January 2027 (commissioning).
P3 Dealer portal. Lead: Marketing manager. Status: not stated as a colour: "On track" (last roll-up: GREEN).
  Reason, as stated: no reason given.
  Moved: design signed off 30 October; build started 2 November.
  End: planned 4 December; lead's forecast 4 December (launch).
P5 Quality system recertification. Lead: Quality manager. Status: not reported (last roll-up: GREEN). End: planned 31 March 2027.

WHERE THE REPORTS DISAGREE OR LEAVE A GAP
Contradictions: 2
  C1. P1 and P3: the date the ERP's customer and price data reach the dealer portal. P1 report: "ready for the dealer portal team from 7 December (was 23 November)" P3 report: "We connect to the ERP's customer and price data from 23 November, as agreed with IT" Not settled here. Ask: IT manager, Marketing manager.
  C2. P2 and P4: when the old warehouse bay is cleared. P2 report: "installation starts on 1 December in the old warehouse bay, once the warehouse move has cleared it" P4 report: "The move out of the old bay therefore finishes on 11 December" Not settled here. Ask: Plant engineer, Logistics manager.
Other gaps: 4
  P2: colour changed from last period's, with no reason given. AMBER last period, GREEN now. Ask: Plant engineer.
  P3: status not stated as a colour. The report says "On track". Ask: Marketing manager.
  P5: no report received. GREEN last period. Ask: Quality manager.
  D2: carried decision that no report or decision note mentions this period. Needed by 6 November. Ask: IT manager.

FOR THE HEAD OF OPERATIONS ONLY. Remove before sending.
To chase before the meeting: 5 people
  IT manager: C1, the date the data reach the portal; D2, not mentioned this period.
  Plant engineer: C2, the date the old bay is cleared; P2's reason for green.
  Marketing manager: C1; P3's status as red, amber or green.
  Logistics manager: C2.
  Quality manager: P5's report for this period.
Left out of the page: 1. A remark judging a person (the ERP supplier's consultant), from the P1 report.
Every status checked against its report as written: [ ]
Confirmed by: [ ]  Date: [ ]
Nothing has been sent, and no status, plan or record has been changed.
```

The page, from the title line to the last gap, came to 797 words, inside the default limit of 800. No "Moved" line needed shortening first.

## What was observed

- **Every required part was produced:** the header, at a glance, the decisions (three, with D1 listed as answered), five project lines in the fixed order, two contradictions, four other gaps, the head of operations' part and the confirmation lines.
- **Nothing made the assistant stop.** The register headings matched, no row repeated an ID, and there were reports and a period. The remark about the supplier's consultant, in the P1 report, was left out of the reason and noted.
- **Statuses, counts, D-numbers, contradictions and gaps matched the published example.** Same five statuses (P3 shown as "On track", not a colour; P5 not reported), same four changes, D2 carried as past the date needed, D3 and D4 numbered on, the same two contradictions (P1 and P3 on the data date; P2 and P4 on when the old bay is clear), the same four gaps, the same five people to chase. No status was worked out or carried forward.
- **Differences from the published example** were all in wording: the report date written without the weekday; the decision questions and the options phrased differently; "End" lines with a short note of what the date is for, in brackets (commissioning, launch, end of the move), which the example leaves out; shorter "Moved" lines in the example; and the note under "Left out of the page", where this run named the subject of the remark (the supplier's consultant) and the example says only that a remark judging a person was left out.
- **Facts not in the inputs:** none that changes anything. Both outputs give "go without them" as the second option on the consultant days; the report implies it ("without them it finishes on 18 December") but does not list it as an option. Both outputs read the dates for commissioning, launch and the end of the warehouse move as the lead's forecast for each project's end, which the reports do not say in those words.
- **The example's closing text overstates one thing.** It says the full page would run over 800 words and so was shortened. This run, written in full, came to 797 words, and the example's own page is 795 words.

## Where the template was ambiguous

1. **A forecast that is an event date.** Step 5 asks for "the lead's forecast for the end date" and says never to work one out. The P2, P3 and P4 reports give a commissioning, launch and move date, not an end date. The run used them and said what they were; the template does not say whether to.
2. **Options that are implied.** Step 6 says options "as given". The P1 decision names one option and the consequence of not taking it. The run turned that into two options. The template does not say whether to do that or to write "none given".
3. **A colour that became a non-colour.** Step 8, gap 5, covers a colour that differs from last period's with no reason. P3 went from GREEN to "On track" with no reason. The run raised only gap 2 (not a colour). It is unclear whether gap 5 also applies.
4. **Numbering several new decisions.** Step 6 numbers new decisions on from the highest D-number but does not say in what order. The run used project ID order.
5. **What "decisions asked" counts.** At a glance counts "decisions asked". The run counted carried decisions as well as new ones. The template does not say.
6. **How much of a left-out remark to name.** The template says to note it under "Left out of the page" and name the report. It does not say whether to name who the remark was about. The run did, and that repeats part of what it was told to leave out.
7. **Merging contradictions.** P3 also launches on 4 December, before the 7 December date P1 gives. The run kept that inside C1. The template does not say whether it is one contradiction or two.
8. **Small points.** The instruction block says "several colours" and the output format says "more than one colour stated". The period in the title line (26 October to 6 November 2026) has no stated date rule. The template does not say whether the weekday goes on the report date.
9. **The acceptance tests** remain unrun. This trial did not run them, and the version notes still say so.

## Changed after this run, and not run again

The output and the observations above are as recorded and describe the template and the example as they stood at the run. On 12 November 2026, after the run was reviewed, these edits were made in response to the findings above:

- **Event dates (ambiguity 1).** Step 5 and the pasted instructions now say that a date given for the event that ends the project is the lead's forecast, shown as the date alone.
- **Implied options (ambiguity 2).** Step 6 and the pasted instructions now say that an alternative the report itself states, such as going without, counts as an option as given. The example's D3 is unchanged.
- **Gap 5 (ambiguity 3).** It now applies only when this period's status is a colour; P3's change to "On track" is raised only as "not stated as a colour".
- **Numbering (ambiguity 4) and the decisions count (ambiguity 5).** New decisions are numbered in project ID order; carried decisions are counted in "decisions asked".
- **One contradiction or two (ambiguity 7).** One disagreement about one fact is one contradiction.
- **Wording and dates (ambiguity 8).** One phrase, "more than one colour stated", throughout; the date rule now gives the form of the period in the title line and says which header dates carry a weekday.
- **The example's closing text.** It no longer says the page was shortened; it states the 795-word count.
- **Left-out remark (ambiguity 6).** The exceptions step and the pasted instructions now say not to say who the remark was about. Not run again.
- **Not changed:** the acceptance tests (ambiguity 9) are still unrun. A clean rerun by a reader who has not seen the output has not been done.
