# Project handover readiness check: an invented example

*Illustrative example with invented data.* The firm, the supplier, the people, the system and every date below are invented. The firm is an invented 90-person building-survey practice. An internal project has replaced its paper and spreadsheet diary with an inspection scheduling system bought from an invented software company, called Supplier A here. The project manager is about to hand the system to the scheduling team, whose manager will run it. People are named by role or by letter. First come the inputs the project manager supplied, in full, then the checklist the capability returned.

## The inputs

### 1. Handover settings

```
Deliverable: Inspection scheduling system
Project manager: Project manager, operations projects
Receiving team: Scheduling team (roles: Scheduling manager, Senior scheduler, Scheduler)
Receiving owner: Scheduling manager
Check date: Thursday 12 November 2026
Planned handover: Monday 16 November 2026
Project team support ends: Friday 11 December 2026
```

### 2. Requirements list (written by the scheduling manager)

```
req_id,area,requirement,must_have,evidence_expected
R01,Acceptance,User acceptance test passed and signed off,yes,sign-off by Scheduling manager
R02,Acceptance,Load test at 400 bookings a day or more,no,test record
R03,Instructions,Daily operating guide for schedulers,yes,document
R04,Instructions,A scheduler has run the morning schedule build from the guide without help,yes,demonstration
R05,Access,Scheduling team holds the access it needs to run and administer the system,yes,access granted
R06,Training,Every scheduler trained and has run a live day unaided,yes,ran unaided
R07,Support,Every support topic has an owner after handover who has agreed to it,yes,owner accepted
R08,Open items,Every open item has an owner after handover and no high-severity item is left without a workaround,yes,owners and workarounds
R09,Instructions,Supplier contacts and escalation route written down,no,document
R10,Support,Response time for system faults agreed with IT,no,service levels confirmed by IT lead
```

### 3. Evidence register

```
ev_id,req_id,description,kind,dated,by
E01,R01,User acceptance test summary: 46 of 48 scripts passed; the 2 failures are logged as OI-02 and OI-03,test record,2026-11-06,Project manager
E02,R01,Sign-off meeting booked for Friday 13 November,note,2026-11-10,Project manager
E03,R02,Load test: 450 simulated bookings in one day with no failed booking,test record,2026-11-04,Supplier A
E04,R03,Daily operating guide version 1.2,document,2026-11-09,Project analyst
E05,R04,Daily operating guide version 1.2 section 2: morning schedule build,document,2026-11-09,Project analyst
E06,R09,Supplier A contacts and escalation route,document,,Project analyst
E07,R10,Message from IT lead: faults reported before 2 pm are answered the same working day,note,2026-11-10,IT lead
E08,,Data move check: 1212 of 1212 open bookings moved from the old diary,test record,2026-11-02,Project analyst
```

### 4. Access list

```
req_id,system,access_level,receiving_holder,status,date
R05,Scheduling system,Scheduler,Scheduling team (4 schedulers),granted,2026-11-02
R05,Scheduling system,Administrator,Scheduling manager,granted,2026-11-02
R05,Scheduling system,Administrator (backup),Senior scheduler,requested,2026-11-09
R05,Supplier A support portal,Named contact,Scheduling manager,not requested,
```

### 5. Training record

```
req_id,person,role,topic,trained_on,ran_unaided_on
R06,Scheduler A,Scheduler,Daily scheduling,2026-10-28,2026-11-03
R06,Scheduler B,Scheduler,Daily scheduling,2026-10-28,2026-11-05
R06,Scheduler C,Scheduler,Daily scheduling,2026-10-29,2026-11-13
R06,Scheduler D,Scheduler,Daily scheduling,,
```

### 6. Support owners

```
req_id,topic,owner_after_handover,accepted,from_date
R07,Day-to-day scheduling questions,Scheduling manager,yes,2026-11-16
R07,System faults and outages,IT lead,yes,2026-11-16
R07,Changes to booking rules and templates,Senior scheduler,no,2026-11-16
R07,Supplier A account and renewals,Operations director,yes,2027-01-04
```

### 7. Open items

```
req_id,item_id,description,severity,workaround,owner_after_handover,due
R08,OI-01,Calendar updates reach inspectors' phones up to 15 minutes late,medium,Inspectors refresh the app before leaving,IT lead,2026-12-04
R08,OI-02,Repeat bookings that fall on a public holiday are not moved,high,Schedulers check holiday weeks by hand (guide section 5),Scheduling manager,2026-11-27
R08,OI-03,Cancellation emails to clients show the old office address,high,,Supplier A,2026-11-20
R08,OI-04,Monthly utilisation report not yet built,low,,,
```

## The output

**HANDOVER READINESS CHECK: Inspection scheduling system**

- **For:** Scheduling manager, Scheduling team. **Prepared by:** Project manager, operations projects.
- **Check date:** Thursday 12 November 2026. **Planned handover:** Monday 16 November 2026. **Project team support ends:** Friday 11 December 2026.
- **Supplied:** requirements (10, 7 must-have); evidence register (8 rows); access list (4 rows); training record (4 rows); support owners (4 rows); open items (4 rows).

**Position by the rules:** 1 of 7 must-have requirements met. Conditions open: 6. For the Scheduling manager to judge: 1. Not must-have and still open: 1. This is a count, not a decision.

**Requirements**

*Acceptance*

- **R01** User acceptance test passed and signed off (must-have). Expected: sign-off by Scheduling manager. **Status: Partly met.** Evidence: E01 test summary, 46 of 48 scripts passed, Friday 6 November; E02 note, sign-off meeting booked for Friday 13 November, Tuesday 10 November (not counted: a note, not a sign-off). Finding: no sign-off by the Scheduling manager; E02 is a note of a meeting, not a sign-off. E01 records 2 failed scripts, logged as OI-02 and OI-03.
- **R02** Load test at 400 bookings a day or more (not must-have). Expected: test record. **Status: Met.** Evidence: E03 load test, 450 simulated bookings in one day with no failed booking, Wednesday 4 November. Finding: nothing missing.

*Instructions*

- **R03** Daily operating guide for schedulers (must-have). Expected: document. **Status: Met.** Evidence: E04 daily operating guide version 1.2, Monday 9 November. Finding: nothing missing.
- **R04** A scheduler has run the morning schedule build from the guide without help (must-have). Expected: demonstration. **Status: Not evidenced.** Evidence: E05 operating guide section 2, Monday 9 November (not counted: a document, not a demonstration). Finding: document only: nobody in the receiving team is recorded doing it.
- **R09** Supplier contacts and escalation route written down (not must-have). Expected: document. **Status: Not evidenced.** Evidence: E06 Supplier A contacts and escalation route (not counted: undated). Finding: E06 is undated.

*Access*

- **R05** Scheduling team holds the access it needs to run and administer the system (must-have). Expected: access granted. **Status: Partly met.** Evidence: access list, 4 rows linked. Finding: 2 of 4 rows granted. Scheduling system, Administrator (backup), Senior scheduler: requested Monday 9 November. Supplier A support portal, Named contact, Scheduling manager: not requested, no date.

*Training*

- **R06** Every scheduler trained and has run a live day unaided (must-have). Expected: ran unaided. **Status: Not met.** Evidence: training record, 4 rows linked. Finding: Scheduler D: not trained. Scheduler C: trained Thursday 29 October; ran unaided dated Friday 13 November, dated after the check date. Schedulers A and B: trained and ran unaided.

*Support*

- **R07** Every support topic has an owner after handover who has agreed to it (must-have). Expected: owner accepted. **Status: Not met.** Evidence: support owners, 4 rows linked. Finding: Changes to booking rules and templates: Senior scheduler named, not accepted. Supplier A account and renewals: cover from Monday 4 January 2027, after the cover limit of Saturday 12 December 2026.
- **R10** Response time for system faults agreed with IT (not must-have). Expected: service levels confirmed by IT lead. **Status: Owner to judge.** Evidence: E07 message from the IT lead, faults reported before 2 pm are answered the same working day, Tuesday 10 November. Finding: the expected evidence is outside the fixed list; for the Scheduling manager to judge.

*Open items*

- **R08** Every open item has an owner after handover and no high-severity item is left without a workaround (must-have). Expected: owners and workarounds. **Status: Not met.** Evidence: open items, 4 rows linked. Finding: OI-03 is high severity with no workaround. OI-04 has no owner after handover.

**Conditions still to meet (proposed)**

- **R01:** The Scheduling manager's sign-off of the user acceptance test is recorded; the test summary shows 2 of 48 scripts failed, logged as OI-02 and OI-03. Owner and date: for the Scheduling manager to set.
- **R04:** Someone in the scheduling team runs the morning schedule build from the guide without help, recorded as a demonstration. Owner and date: for the Scheduling manager to set.
- **R05:** The Senior scheduler's Administrator (backup) access to the scheduling system and the Scheduling manager's named contact on the Supplier A support portal are granted. Owner and date: for the Scheduling manager to set.
- **R06:** Scheduler D is trained, and Schedulers C and D each run a live day unaided. Owner and date: for the Scheduling manager to set.
- **R07:** The Senior scheduler agrees to own changes to booking rules and templates, and Supplier A account and renewals has an agreed owner from Saturday 12 December 2026 to Sunday 3 January 2027. Owner and date: for the Scheduling manager to set.
- **R08:** OI-03 has a workaround, and OI-04 has an owner after handover. Owner and date: for the Scheduling manager to set.

**Also open (not must-have)**

- **R09:** Not evidenced. E06 is undated.

**For the Scheduling manager to judge**

- **R10** Response time for system faults agreed with IT. Expected: service levels confirmed by IT lead. Supplied: E07, a message from the IT lead saying faults reported before 2 pm are answered the same working day, Tuesday 10 November. Question: does this meet the requirement?

**Support after handover**

- Day-to-day scheduling questions: Scheduling manager, accepted, cover from Monday 16 November 2026.
- System faults and outages: IT lead, accepted, cover from Monday 16 November 2026.
- Changes to booking rules and templates: Senior scheduler, named, not accepted, cover from Monday 16 November 2026.
- Supplier A account and renewals: Operations director, accepted, cover from Monday 4 January 2027. Gap: Saturday 12 December 2026 to Sunday 3 January 2027, 23 days.

**Open items carried into operation**

- **OI-02** (high) Repeat bookings that fall on a public holiday are not moved. Workaround: schedulers check holiday weeks by hand (guide section 5). Owner after handover: Scheduling manager. Due: Friday 27 November 2026.
- **OI-03** (high) Cancellation emails to clients show the old office address. Workaround: none. Owner after handover: Supplier A. Due: Friday 20 November 2026.
- **OI-01** (medium) Calendar updates reach inspectors' phones up to 15 minutes late. Workaround: inspectors refresh the app before leaving. Owner after handover: IT lead. Due: Friday 4 December 2026.
- **OI-04** (low) Monthly utilisation report not yet built. Workaround: none. Owner after handover: not assigned. Due: not stated.

**Supplied but not linked**

- E08: data move check, 1212 of 1212 open bookings moved from the old diary, Monday 2 November. No requirement named.

**Decision of the Scheduling manager (left blank for them)**

[ ] Accept the handover   [ ] Accept with the conditions above   [ ] Not accepted yet

Name, role and date: ____________

Prepared for the Scheduling manager's decision. Nothing has been granted, removed, signed, sent or changed.
