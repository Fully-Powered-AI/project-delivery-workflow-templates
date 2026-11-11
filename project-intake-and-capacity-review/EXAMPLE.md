# Project intake and capacity review: an invented example

*Illustrative example with invented data.* The business, its people, its projects, the proposal and every figure below are invented. The business is an invented 40-person web and brand agency. The operations lead runs the review for the managing director, who owns the portfolio and decides. People are named by role only. First come the five inputs the operations lead supplied, in full, then the review the capability returned.

## The inputs

### 1. Settings

```
Portfolio owner: Managing director
Review date: Tuesday 10 November 2026
Months: 2027-01 to 2027-04
Load ceiling: 85%
Scale: 1 to 5 on every criterion

Criteria and weights (total 100):
Value (40): 1 no benefit stated; 2 benefit named but not sized; 3 sized by
  the proposer's estimate only; 4 sized from the agency's own records;
  5 sized from records and worth over $50,000 a year
Strategic fit (30): 1 none of this year's goals; 2 touches a goal in
  passing; 3 supports one goal indirectly; 4 supports one goal directly;
  5 supports two goals directly
Urgency (20): 1 no date; 2 a wished-for date, no consequence of missing it
  stated; 3 a date with a stated cost of missing it; 4 as 3, and the date
  is within three months of the start; 5 an external fixed date
Confidence (10): 1 no estimate of effort; 3 effort estimated by the
  proposer; 5 effort estimated by the roles that would do it

This year's goals: G1 keep and grow retained clients; G2 cut delivery
overhead; G3 launch two new service lines.
```

### 2. Committed projects (exported from the portfolio sheet)

```
ID,Project,Start,End,Fixed,Value,Strategic fit,Urgency,Confidence
P1,Client portal rebuild,2027-01,2027-04,No,4,5,3,4
P2,Annual brand refresh,2027-01,2027-04,No,3,3,2,5
P3,Billing system migration,2027-01,2027-04,Yes,3,4,5,4
P4,Careers site update,2027-02,2027-03,No,2,2,2,4
```

### 3. Delivery days used by committed projects

```
ID,Role,2027-01,2027-02,2027-03,2027-04
P1,Designer,10,10,8,0
P1,Developer,30,30,25,15
P1,Project manager,6,6,5,3
P2,Designer,15,20,20,5
P2,Developer,0,5,5,0
P2,Project manager,4,4,4,2
P3,Developer,20,20,20,20
P3,Project manager,6,6,6,6
P4,Designer,0,8,8,0
P4,Developer,0,10,5,0
P4,Project manager,0,2,2,0
```

### 4. Days available by role (after leave and run work)

```
Role,2027-01,2027-02,2027-03,2027-04
Designer,60,60,60,60
Developer,80,80,70,80
Project manager,40,40,40,40
```

### 5. The proposal

```
Proposal: Customer self-service booking tool
Proposed by: Client services lead
Wanted start: 2027-01, three months
What it is: A page where retained clients book their monthly review
  meetings and check delivery dates themselves.
Why: In October the client services lead counted 46 email threads in the
  shared booking inbox that existed only to arrange a review meeting, about
  20 minutes each, handled by the project managers. Three retained clients have asked for a
  booking page. The lead would like it live before the May booking
  season; nothing is stated about what happens if it is late.
Effort (the client services lead's own estimate, not checked with the
  delivering roles):
Role,Month 1,Month 2,Month 3
Designer,10,12,5
Developer,25,25,20
Project manager,5,5,4
```

## The review the capability returned

**Project intake and capacity review: Customer self-service booking tool**

- **For:** Managing director, as portfolio owner. Review date 10 November 2026. Months 2027-01 to 2027-04. Ceiling 85%. Criteria as supplied; ceiling as supplied.
- **The proposal in brief:** Proposed by the client services lead. A page where retained clients book their monthly review meetings and check delivery dates. Wanted start 2027-01 for three months. Stated reason: 46 booking email threads in the shared booking inbox in October, about 20 minutes each, and three retained clients have asked. Effort figures are the proposer's own estimate.
- **Score beside the committed projects:** Proposed scores, for the managing director to confirm or change. Ranked by weighted score, out of 5.
  1. P1 Client portal rebuild: 4.10 (Value 4, Strategic fit 5, Urgency 3, Confidence 4).
  2. P3 Billing system migration: 3.80 (3, 4, 5, 4). Fixed.
  3. Proposal, Customer self-service booking tool: 3.50 (4, 4, 2, 3). Proposed. Third of five.
  4. P2 Annual brand refresh: 3.00 (3, 3, 2, 5).
  5. P4 Careers site update: 2.20 (2, 2, 2, 4).
  Evidence for the proposed scores:
  - Value 4: "counted 46 email threads in the shared booking inbox that existed only to arrange a review meeting, about 20 minutes each" is a count taken from the agency's own records, and no yearly figure over $50,000 is stated.
  - Strategic fit 4: "Three retained clients have asked for a booking page" and "A page where retained clients book their monthly review meetings" tie it directly to G1, keep and grow retained clients. The proposal claims no saving in delivery overhead, so G2 is not counted as directly supported; one goal directly is a 4.
  - Urgency 2: "would like it live before the May booking season" is a wished-for date, and "nothing is stated about what happens if it is late."
  - Confidence 3: "the client services lead's own estimate, not checked with the delivering roles."
- **Monthly load by role:** Days, with the share of available days. Committed, then with the proposal, against the ceiling in days.
  - Designer, 2027-01: capacity 60.0; committed 25.0 (41.7%); with proposal 35.0 (58.3%); ceiling 51.0; 16.0 days of room.
  - Designer, 2027-02: capacity 60.0; committed 38.0 (63.3%); with proposal 50.0 (83.3%); ceiling 51.0; 1.0 days of room.
  - Designer, 2027-03: capacity 60.0; committed 36.0 (60.0%); with proposal 41.0 (68.3%); ceiling 51.0; 10.0 days of room.
  - Designer, 2027-04: capacity 60.0; committed 5.0 (8.3%); with proposal 5.0 (8.3%); ceiling 51.0; 46.0 days of room.
  - Developer, 2027-01: capacity 80.0; committed 50.0 (62.5%); with proposal 75.0 (93.8%); ceiling 68.0; over the ceiling by 7.0 days.
  - Developer, 2027-02: capacity 80.0; committed 65.0 (81.3%); with proposal 90.0 (112.5%); ceiling 68.0; over the ceiling by 22.0 days.
  - Developer, 2027-03: capacity 70.0; committed 55.0 (78.6%); with proposal 75.0 (107.1%); ceiling 59.5; over the ceiling by 15.5 days.
  - Developer, 2027-04: capacity 80.0; committed 35.0 (43.8%); with proposal 35.0 (43.8%); ceiling 68.0; 33.0 days of room.
  - Project manager, 2027-01: capacity 40.0; committed 16.0 (40.0%); with proposal 21.0 (52.5%); ceiling 34.0; 13.0 days of room.
  - Project manager, 2027-02: capacity 40.0; committed 18.0 (45.0%); with proposal 23.0 (57.5%); ceiling 34.0; 11.0 days of room.
  - Project manager, 2027-03: capacity 40.0; committed 17.0 (42.5%); with proposal 21.0 (52.5%); ceiling 34.0; 13.0 days of room.
  - Project manager, 2027-04: capacity 40.0; committed 11.0 (27.5%); with proposal 11.0 (27.5%); ceiling 34.0; 23.0 days of room.
- **Over the ceiling, and what would have to give way:** Three role-months, all Developer. Running totals assume the whole month's days of a project are released; releasing part is the managing director's call.
  - Developer, 2027-01: over by 7.0 days. Fixed work that cannot move: P3, 20.0 days. Committed work using this role, lowest score first: P1 Client portal rebuild, 4.10, 30.0 days (running total 30.0). The 7.0 days are covered only when P1 is included. P1 and P3 score higher than the proposal.
  - Developer, 2027-02: over by 22.0 days. Fixed work that cannot move: P3, 20.0 days. Committed work, lowest score first: P4 Careers site update, 2.20, 10.0 days (10.0); P2 Annual brand refresh, 3.00, 5.0 days (15.0); P1 Client portal rebuild, 4.10, 30.0 days (45.0). The 22.0 days are covered only when P1 is included. P4 and P2 score lower than the proposal; P1 and P3 score higher.
  - Developer, 2027-03: over by 15.5 days. Fixed work that cannot move: P3, 20.0 days. Committed work, lowest score first: P4 Careers site update, 2.20, 5.0 days (5.0); P2 Annual brand refresh, 3.00, 5.0 days (10.0); P1 Client portal rebuild, 4.10, 25.0 days (35.0). The 15.5 days are covered only when P1 is included. P4 and P2 score lower than the proposal; P1 and P3 score higher.
- **Start months tested:** Only starts whose three months all fall inside the supplied months can be tested.
  - Start 2027-01 (months 2027-01 to 2027-03): over the ceiling in Developer in all three months, as above.
  - Start 2027-02 (months 2027-02 to 2027-04): Developer over the ceiling in 2027-02 (by 22.0 days) and 2027-03 (by 20.5 days); 2027-04 fits, with 13.0 days of room. Designer and Project manager fit in all three months.
  - Starts from 2027-03: not tested. Capacity for months after 2027-04 was not supplied.
  - Developer room under the ceiling before the proposal, against what the proposal asks, for a 2027-01 start: 18.0 against 25.0 (2027-01), 3.0 against 25.0 (2027-02), 4.5 against 20.0 (2027-03).
- **Gaps and questions:**
  1. The effort figures are the proposer's estimate. Ask the Designer, Developer and Project manager roles to confirm or correct them.
  2. Is the May booking season a date with a cost if missed? If so, Urgency would rise from 2.
  3. Does the proposal claim a saving in delivery overhead (G2)? Nothing is stated; if the portfolio owner counts it as a direct saving, Strategic fit would be 5.
  4. Capacity for 2027-05 onward was not supplied, so a later start cannot be tested. Supply it if deferral is considered.
  5. Are the four proposed scores accepted as they stand?
- **Decision for the Managing director: accept, defer or reject.** Nothing here is a recommendation.
  - Facts if accepted at a 2027-01 start: Developer is over the ceiling in three months, by 7.0, 22.0 and 15.5 days. The only way to cover the gap in 2027-02 and 2027-03 from committed work includes P1, which scores higher than the proposal. P3 is fixed.
  - Facts if deferred: a 2027-02 start still leaves Developer over the ceiling in two months. A start from 2027-03 cannot be tested without capacity after April.
  - Facts if rejected: the proposal ranks third of five at 3.50, above P2 and P4. Its Urgency is 2 and its effort is unconfirmed.

Every figure traces to the inputs supplied. The review changes no plan, schedules nothing and tells no one.
