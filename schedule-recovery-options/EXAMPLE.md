# Schedule recovery options: an invented example

*Illustrative example with invented data.* Company A is an invented 45-person services firm replacing its booking and invoicing system. Every name, role, date and figure below is made up, and Vendor B is an invented supplier. The inputs come first, in full, then the page the assistant produces from them.

## The inputs

**The slip note, from the Data lead, Wednesday 16 June 2027:** "The migration rehearsal found about 1,400 duplicate customer rows. Cleaning them means a second rehearsal. I now expect the rehearsal to be complete on Friday 2 July, not Friday 18 June." The project manager adds: the sponsor is the Managing director; delivery leads are the Test lead, Training lead and Operations lead; the Finance lead confirms any deferral that affects Finance. The monthly report that the Reports module produces is Finance's, and Finance makes it today from the spreadsheet export.

**The schedule export** (plan not yet changed for the slip):

```
ID,Task,Type,Owner,Start,Finish,Baseline Finish,Duration (wd),Remaining (wd),Predecessors,Committed To
M1,Migration rehearsal complete,Milestone,Data lead,2027-06-18,2027-06-18,2027-06-18,0,0,,Sponsor
T1,User acceptance testing (UAT),Task,Test lead,2027-06-21,2027-07-02,2027-07-02,10,10,M1,
T2,Staff training,Task,Training lead,2027-07-05,2027-07-09,2027-07-09,5,5,T1,
T3,Cutover preparation,Task,Operations lead,2027-07-12,2027-07-16,2027-07-16,5,5,T2,
M2,Go-live,Milestone,Operations lead,2027-07-19,2027-07-19,2027-07-19,0,0,T3,Operations staff
M3,Hypercare ends,Milestone,Operations lead,2027-07-30,2027-07-30,2027-07-30,0,0,M2,Sponsor
M4,Old system licence ends,Milestone,Sponsor,2027-08-31,2027-08-31,2027-08-31,0,0,,Old system supplier
```

**Estimates and flexibility, from the delivery leads:**

```
ID,People Now,Person-Days Remaining,Can Be Split,Can Start Before Predecessor Ends (wd),Note
T1,2,20,yes,0,"Three modules tested one after another: Booking 4 wd, Invoicing 3 wd, Reports 3 wd"
T2,1,5,no,0,
T3,1,5,no,3,"First 3 working days (runbook, rollback plan, access list) do not need training to finish. Operations lead."
```

**The scope list:**

```
Item,Priority,Effort (wd),If Deferred,Task
Booking module,Must,4,Cannot defer,T1
Invoicing module,Must,3,Cannot defer,T1
Reports module,Should,3,"Monthly report from the spreadsheet export, as done today",T1
```

**Who could help:**

```
Person or Role,Available From,Available Until,Days per Week,Can Join
Tester from the Support team,2027-07-05,2027-07-23,5,T1
```

The Support team lead has said the tester is free "if asked". Nobody has asked.

**Outside commitments:**

```
Dependency,Supplier,Needed For,Committed Date,Accepted,Notice to Change (wd)
Go-live support on site,Vendor B,M2,2027-07-19 to 2027-07-20,yes,10
```

**Fixed dates and settings:**

- The old system licence ends Tuesday 31 August 2027 and cannot be moved.
- Finance quarter-end close, Monday 2 August to Friday 6 August 2027: no go-live inside it. Accepted by the Finance lead.
- Today is Wednesday 16 June 2027. The schedule export was taken the same day, before the slip was entered. Operations staff were told go-live on Monday 19 July; nobody else is recorded as told.
- Working calendar: Monday to Friday. Company A observes no holidays between 21 June and 31 August.
- Go-live is the working day after cutover preparation ends. Hypercare is 10 working days counted from go-live day. A newcomer needs 3 working days before they help. Up to 4 options.

## The page the assistant produces

```
SCHEDULE RECOVERY OPTIONS: Migration rehearsal complete (M1)

For: Managing director. Dates to be confirmed by: Test lead, Training lead, Operations lead (Finance lead for any deferral). Prepared Wed 16 Jun 2027 from the schedule export of Wed 16 Jun 2027.

The slip: M1 was committed for Fri 18 Jun and is now forecast for Fri 2 Jul, 10 working days late. Cause as reported: about 1,400 duplicate customer rows found in the rehearsal; a second rehearsal is needed. The forecast is the Data lead's single estimate; no range was given.

If nothing changes: Go-live (M2) moves from Mon 19 Jul to Mon 9 Aug, 15 working days late. The chain runs UAT Mon 5 to Fri 16 Jul, training Mon 19 to Fri 23 Jul, cutover preparation Mon 26 to Fri 30 Jul. The next working day, Mon 2 Aug, falls inside Finance's close (2 to 6 Aug, no go-live), so the date moves to Mon 9 Aug. Later milestones: Hypercare ends (M3) Fri 20 Aug, 7 working days before the licence ends on Tue 31 Aug (M4). Dependencies hit: Vendor B's on-site support is accepted for 19 and 20 Jul only; nothing is accepted for 9 Aug, and the latest date to ask for a change is Mon 26 Jul (10 working days' notice). Already told the current date: Operations staff (Mon 19 Jul). No other audience is recorded.

Options: 4

Option 1: Defer the Reports module
- Change: UAT covers Booking and Invoicing only; Reports (Should, 3 working days) is deferred with no new date. UAT falls from 10 to 7 working days.
- Takes out of the chain: 3 working days.
- Dates after: UAT Mon 5 to Tue 13 Jul; training Wed 14 to Tue 20 Jul; cutover preparation Wed 21 to Tue 27 Jul.
- Go-live: Wed 28 Jul, 7 working days after the committed date (8 fewer than if nothing changes).
- Later milestones: Hypercare ends Tue 10 Aug, 15 working days before the licence ends; hypercare covers Finance's close week.
- Dependencies: Vendor B support for Wed 28 Jul is not accepted; latest date to ask Wed 14 Jul (10 working days' notice). No request is recorded.
- Rests on: the Data lead's date of Fri 2 Jul holding; the fallback being acceptable (Finance makes the monthly report from the spreadsheet export, as done today); the Test lead's estimates for the other two modules holding.
- Costs: the Reports module has no date and needs its own decision. Finance makes the monthly report from the spreadsheet export until then.
- Confirm with: Test lead (UAT dates); Finance lead (the fallback, since the monthly report is Finance's).

Option 2: Start cutover preparation during training
- Change: cutover preparation starts on the third day of training, not after it ends.
- Takes out of the chain: 3 working days.
- Dates after: UAT Mon 5 to Fri 16 Jul; training Mon 19 to Fri 23 Jul; cutover preparation Wed 21 to Tue 27 Jul.
- Go-live: Wed 28 Jul, 7 working days after the committed date (8 fewer than if nothing changes).
- Later milestones: Hypercare ends Tue 10 Aug, 15 working days before the licence ends; hypercare covers Finance's close week.
- Dependencies: Vendor B support for Wed 28 Jul is not accepted; latest date to ask Wed 14 Jul. No request is recorded.
- Rests on: the Operations lead's note that the first 3 working days of preparation (runbook, rollback plan, access list) do not need training to finish; M1 finishing on its forecast of Fri 2 Jul; UAT finishing on its forecast.
- Costs: None stated in the inputs.
- Confirm with: Operations lead (overlap and dates); Training lead (training dates).

Option 3: Add one tester to UAT
- Change: a tester from the Support team joins UAT from Mon 5 Jul. UAT is 20 person-days; with three people and a 3-day start-up, the task takes 8 working days, not 10 ((20 + 3) / 3 = 7.67, rounded up).
- Takes out of the chain: 2 working days.
- Dates after: UAT Mon 5 to Wed 14 Jul; training Thu 15 to Wed 21 Jul; cutover preparation Thu 22 to Wed 28 Jul.
- Go-live: Thu 29 Jul, 8 working days after the committed date (7 fewer than if nothing changes).
- Later milestones: Hypercare ends Wed 11 Aug, 14 working days before the licence ends; hypercare covers Finance's close week.
- Dependencies: Vendor B support for Thu 29 Jul is not accepted; latest date to ask Thu 15 Jul. No request is recorded.
- Rests on: UAT work dividing evenly across three testers (the Test lead marked it splittable); the newcomer adding nothing for 3 working days; the Data lead's date of Fri 2 Jul holding; the Support team lead releasing the tester, who has not yet been asked.
- Costs: one Support tester for 8 working days (5 to 14 Jul).
- Confirm with: Test lead (the task can be split, and the dates); Support team lead (release of the tester).

Option 4: Move go-live to Mon 9 Aug
- Change: no change to scope, order or people. Go-live is reset to Mon 9 Aug, the first allowed working day. The dates equal the do-nothing dates; the difference is that the commitment is re-baselined to Mon 9 Aug.
- Takes out of the chain: 0 working days.
- Dates after: UAT Mon 5 to Fri 16 Jul; training Mon 19 to Fri 23 Jul; cutover preparation Mon 26 to Fri 30 Jul.
- Go-live: Mon 9 Aug, 15 working days after the committed date (the same as if nothing changes).
- Later milestones: Hypercare ends Fri 20 Aug, 7 working days before the licence ends. The date holds if cutover preparation finishes by Fri 6 Aug, so it absorbs up to 5 working days of further slip.
- Dependencies: Vendor B support for Mon 9 Aug is not accepted; latest date to ask Mon 26 Jul. No request is recorded.
- Rests on: the Data lead's date of Fri 2 Jul holding; Finance's close staying 2 to 6 Aug.
- Costs: Operations staff were told Mon 19 Jul; they would need a new date. Full scope is kept.
- Confirm with: Operations lead (dates); Finance lead (close week).

Combinations: Options 1 and 2 together take out 6 working days: UAT Mon 5 to Tue 13 Jul; training Wed 14 to Tue 20 Jul; cutover preparation Fri 16 to Thu 22 Jul; go-live Fri 23 Jul, 4 working days after the committed date; hypercare ends Thu 5 Aug, 18 working days before the licence ends; Vendor B latest date to ask Fri 9 Jul. Options 1, 2 and 3 together take out 7, not 8, because Option 3 saves only 1 more day once the Reports module is gone (its 3 working days on 2 people are 6 person-days, so 14 remain; with three testers, (14 + 3) / 3 = 5.67, 6 working days): UAT Mon 5 to Mon 12 Jul; training Tue 13 to Mon 19 Jul; cutover preparation Thu 15 to Wed 21 Jul; go-live Thu 22 Jul, 3 working days after the committed date; hypercare ends Wed 4 Aug, 19 working days before the licence ends; Vendor B latest date to ask Thu 8 Jul. No option restores Mon 19 Jul.

Not known: (1) Whether Finance accepts its 2 to 6 Aug close falling inside hypercare under Options 1 to 3; the inputs say only that go-live may not fall in it: Finance lead. (2) Whether Vendor B can support any date other than 19 and 20 Jul; no request is recorded: Operations lead. (3) Whether the Support team lead will release a tester: Support team lead. (4) Whether anyone beyond Operations staff was told Mon 19 Jul: project manager. (5) Whether any person is needed both in the first days of training and in the first 3 days of cutover preparation: Training lead and Operations lead.

Decision for the Managing director: choose one option or combination; the Test lead, Training lead and Operations lead confirm each date. Working days counted Monday to Friday; holidays used: none. Nothing is changed in the plan, promised to anyone or sent.
```
