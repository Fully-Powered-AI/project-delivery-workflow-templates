# Project handover readiness check

Workflow template, version 0.1.0.

## Purpose

Prepare the handover checklist a project manager takes to the owner of the team that will run a finished deliverable. Every requirement the receiving team has written down is checked against what the project has actually supplied: acceptance evidence, operating instructions, access, training, support owners and open items. Each requirement gets a status by fixed rules, every shortfall is stated as a fact, and each unmet must-have becomes a proposed condition. The receiving owner then accepts the handover, accepts it with conditions, or declines it for now. The assistant prepares; it never grants or removes access, signs anything off, assigns an owner, sets a date, sends the checklist or decides whether the handover is accepted.

## When to use it and when not to

Use it when a project's deliverable, such as a new system, a rebuilt process, a fitted-out site or a reporting tool, is due to pass from the project team to the team that will run it day to day. Run it a few working days before the planned handover, so there is time to close the gaps, and again on the day.

Do not use it:

- when a person leaves or changes role and hands over their own work. That is employee offboarding, with its own checklist;
- when a sale closes and the account passes from sales to the client team. That is an account handoff;
- to write the operating procedure itself. Writing down how the work is done is a separate workflow template; this one only checks that the procedure exists and has been used;
- to close the project. Closing it, and agreeing what obligations survive it, is the sponsor's separate step after the handover is accepted;
- to decide what a supplier agreement, warranty or service commitment obliges anyone to do. The person who manages that agreement answers it;
- when the receiving team has written no requirements. The receiving owner writes them first.

## Roles

- **Runs it:** the project manager handing over the deliverable.
- **Writes the requirements and decides on the handover:** the receiving owner, the person accountable for running the deliverable once it is handed over.
- **Grants access, confirms training, accepts support topics:** the system owners, trainers and support owners named in the registers. Always people.
- **Owns each condition after the decision:** whoever the receiving owner names.
- **Closes the project afterwards:** the sponsor, separately.

## Inputs

The person supplies these as files or pasted tables. The assistant needs no connection to any system and never asks for a password, a login code or any other secret.

1. **Handover settings.** The deliverable's name; the project manager's role; the receiving team and its roles; the receiving owner's role; the check date (today); the planned handover date; and the date the project team's own support ends, if it continues for a period after handover. If the deliverable, the receiving owner, the receiving team's roles, the check date or the planned handover date is missing, stop and ask.
2. **Requirements list,** written by the receiving owner. Default headings: `req_id, area, requirement, must_have, evidence_expected`. Area is one of Acceptance, Instructions, Access, Training, Support, Open items. Must-have is yes or no. Evidence expected is one of the words in procedure step 5; any other wording is allowed and is handed to the receiving owner to judge. If there is no list, stop.
3. **Evidence register,** kept by the project manager. Default headings: `ev_id, req_id, description, kind, dated, by`. Kind is one of sign-off, test record, document, demonstration, note. If not supplied, write "not supplied" in the header and continue.
4. **Access list.** Default headings: `req_id, system, access_level, receiving_holder, status, date`. Status is granted, requested or not requested. It records who holds what, never how to sign in. If not supplied, write "not supplied" and continue.
5. **Training record.** Default headings: `req_id, person, role, topic, trained_on, ran_unaided_on`. Ran unaided means the person has done the work for real without help. If not supplied, write "not supplied" and continue.
6. **Support owners.** Default headings: `req_id, topic, owner_after_handover, accepted, from_date`. Accepted is yes or no: yes only when the owner has agreed, not when a plan names them. If not supplied, write "not supplied" and continue.
7. **Open items.** Defects, known issues and unfinished work. Default headings: `req_id, item_id, description, severity, workaround, owner_after_handover, due`. Severity is high, medium or low. If not supplied, write "not supplied" and continue.

If a file's headings do not match the defaults, in any order, stop and ask which column is which. Never guess a column.

## The procedure

1. **Check the inputs.** Confirm the settings named in input 1. Confirm each file's headings. Count the requirements and the must-haves, and the rows in each register. If two requirements share a `req_id`, or two rows share an `ev_id` or an `item_id`, stop and ask. If a requirement's area is not one of the six, stop and ask which it is. If a must-have value is neither yes nor no, treat it as yes and say so in that requirement's finding.
2. **Look for secrets.** If any file holds a password, a login code, a key or a similar secret, stop. Do not repeat it. Ask for the file again without it, and tell the person to let the system's owner know it was written down.
3. **Link every row.** Each register row answers the requirement its `req_id` names. A row with a blank `req_id`, or one that is not on the requirements list, is never dropped: it goes under "Supplied but not linked".
4. **Count only what has happened.** A date later than the check date is planned, not done, and does not count; the finding says "dated after the check date". This applies to the evidence register's dated, the access list's date for a granted row, and the training record's trained_on and ran_unaided_on. It does not void a support owner's from_date, which is compared with the cover limit, or an open item's due, which is only shown. A blank date where the rule needs one does not count; the finding says "undated" or "not trained", as fits.
5. **Give each requirement a status** from its expected evidence. Only rows from the register named here count; any linked row that does not count (the wrong kind or register, undated, or dated after the check date) is listed under Evidence, marked "(not counted: [why, in a few words])".
   - **sign-off by [role]** (evidence register): Met if a counted row of kind sign-off is by that role. Partly met if there is no such sign-off but a counted test record is linked. Not evidenced otherwise. A sign-off by a different role does not count, and the finding names who signed.
   - **test record** (evidence register): Met if a counted row of kind test record is linked. Not evidenced otherwise.
   - **document** (evidence register): Met if a counted row of kind document is linked. Not evidenced otherwise.
   - **demonstration** (evidence register): Met if a counted row of kind demonstration is by one of the receiving team's roles. A document or a note alone leaves it Not evidenced, with the finding "document only: nobody in the receiving team is recorded doing it". A demonstration by the project team leaves it Not evidenced, with the finding "shown by the project team, not by the receiving team".
   - **access granted** (access list): Met if every linked row is granted and counted. Not met if none is. Partly met otherwise. If the access list holds no row linked to the requirement, it is Not evidenced. A row that stands for a group of people counts as one row. The finding gives how many rows are granted and each row that is not, with its status and date, or "no date" when it has none.
   - **ran unaided** (training record): Not met if any linked person has no counted trained date. Otherwise Partly met if any has no counted ran-unaided date. Otherwise Met. If the training record holds no row linked to the requirement, it is Not evidenced. The finding names each person who falls short and why.
   - **owner accepted** (support owners): Not met if any linked row is not accepted. Otherwise Partly met if any owner's cover starts after the cover limit. Otherwise Met. If the support owners register holds no row linked to the requirement, it is Not evidenced. If a requirement is Not met for one reason and another also applies, such as a row not accepted and cover that starts after the cover limit, the finding names every reason that applies. The cover limit is the day after the project team's support ends or, when no end date is given, the planned handover date.
   - **owners and workarounds** (open items): Not met if any linked item has no owner after handover, or any high-severity item has no workaround. Otherwise Met. If the open items list was supplied and holds no items, Met, with the finding "no open items listed".
   - **Any other wording:** Owner to judge. Show what was supplied; do not decide whether it is enough.
   - **No counted row of the right register:** Not evidenced, unless a rule above says otherwise. For the access granted, ran unaided and owner accepted rules, a requirement with no linked row in the named register is Not evidenced, never Met or Not met.
   - **Content that falls short:** where the requirement states a figure or a result and a counted row's own description shows less, such as failed test scripts against "passed", the status is no better than Partly met, and the finding gives both. Whether a document's content is good enough is for the receiving owner; the status says only that the right kind of evidence exists.
6. **Write each finding in facts:** the row ids, dates and fields that fall short. Print the requirements by area in the fixed order (Acceptance, Instructions, Access, Training, Support, Open items) and in the order supplied within each area. For Met, write "nothing missing". Never rate a person's ability; report only the dates supplied.
7. **Support cover.** For each support row, give the topic, the owner, whether they have accepted, and the date their cover starts. When cover starts after the cover limit, state the gap: from the day after the project team's support ends to the day before cover starts, and its length in calendar days. When the project team's support end is not stated, the gap runs from the planned handover date.
8. **Open items.** List every open item, high severity first, then medium, then low, in the order supplied within each. Write "none", "not assigned" or "not stated" for a blank field.
9. **Conditions.** Each must-have whose status is Partly met, Not met or Not evidenced becomes one proposed condition, written as what must be true for the requirement to be met, built only from its finding. Leave the owner and the date for the receiving owner to set. Requirements that are not must-haves and are not Met or Owner to judge go under "Also open". Every Owner to judge requirement, must-have or not, goes under "For the receiving owner to judge", with a question asking whether what was supplied meets it.
10. **Position line.** Count the must-haves that are Met, the conditions open, the requirements for the receiving owner to judge, and the requirements that are not must-haves and appear under Also open (an Owner to judge requirement is counted only under the owner's judgement). It is a count, not a recommendation.
11. **Leave the decision blank.** Print the decision block unfilled. Return the checklist to the project manager, who shares it with the receiving owner. Nothing is sent by the assistant.

## Exceptions and stop conditions

- **No requirements list:** stop. Never supply a standard list. You may name the six areas and the expected-evidence words so the receiving owner can write one.
- **A required setting missing, headings that do not match, a repeated id or an unknown area:** stop and ask, naming exactly what is missing or which file it is in.
- **A password, login code, key or other secret in any file:** stop; do not repeat it; ask for the file again without it.
- **Asked to grant or remove access, mark a requirement met, record a sign-off, accept a support topic for someone, set an owner or a date for a condition, or decide whether to accept the handover:** decline and name the role that does it.
- **Asked to send the checklist or update a project or service record:** decline; the project manager does that after the receiving owner has seen it.
- **Asked what a supplier agreement, warranty or service commitment requires:** decline; that question goes to the person who manages the agreement.
- **A training or support row gives a personal reason, such as illness or leave, for a missing date:** do not repeat the reason; report only that the date is missing.
- **The evidence register says a requirement is met but gives no dated row:** follow the rules; a statement that something is done is a note, not evidence.

## Output format

```
HANDOVER READINESS CHECK: [deliverable]

For: [receiving owner role], [receiving team]. Prepared by: [project manager role].
Check date: [weekday date]. Planned handover: [weekday date]. Project team support ends: [weekday date / not stated].
Supplied: requirements ([n], [n] must-have); evidence register ([n] rows / not supplied); access list ([n] rows / not supplied); training record ([n] rows / not supplied); support owners ([n] rows / not supplied); open items ([n] rows / not supplied).

Position by the rules: [n] of [n] must-have requirements met. Conditions open: [n]. For the [receiving owner role] to judge: [n]. Not must-have and still open: [n]. This is a count, not a decision.

Requirements

Acceptance
[req_id] [requirement] ([must-have / not must-have]). Expected: [evidence expected]. Status: [Met / Partly met / Not met / Not evidenced / Owner to judge]. Evidence: [evidence rows by id, each with a few words and its date, and "(not counted: [why])" on a linked row that does not count / the register and how many rows are linked / none]. Finding: [the shortfall in facts / nothing missing].
[An area with no requirements: No requirements in this area.]

Instructions
[as above]

Access
[as above]

Training
[as above]

Support
[as above]

Open items
[as above]

Conditions still to meet (proposed)
[req_id]: [what must be true for the requirement to be met]. Owner and date: for the [receiving owner role] to set.
[None.]

Also open (not must-have)
[req_id]: [status]. [The shortfall.]
[None.]

For the [receiving owner role] to judge
[req_id] [requirement]. Expected: [as written]. Supplied: [row ids, with what each says / nothing]. Question: does this meet the requirement?
[None.]

Support after handover
[Topic]: [owner / not assigned], [accepted / named, not accepted], cover from [weekday date / not stated]. [Gap: [weekday date] to [weekday date], [n] days.]
[No support owners supplied.]

Open items carried into operation
[item_id] ([severity]) [description]. Workaround: [text / none]. Owner after handover: [role / not assigned]. Due: [weekday date / not stated].
[No open items listed. / Open items list not supplied.]

Supplied but not linked
[row id or register and row number]: [a few words, date]. [No requirement named / Names [req_id], which is not on the requirements list.]
[None.]

Decision of the [receiving owner role] (left blank for them)
[ ] Accept the handover   [ ] Accept with the conditions above   [ ] Not accepted yet
Name, role and date: ____________

Prepared for the [receiving owner role]'s decision. Nothing has been granted, removed, signed, sent or changed.
```

## Reviewer checklist

1. Every requirement on the list appears once, in its area, with its wording unchanged. (Project manager)
2. Every status follows the rule for its expected evidence, and nothing dated after the check date has been counted. (Project manager)
3. No requirement that expects a demonstration is Met on a document, and the receiving owner has opened each document counted as Met and agrees it is the right one. (Receiving owner)
4. Every support owner shown as accepted has in fact agreed, and every gap's dates and day count are right. (Receiving owner)
5. Every open item appears, high severity first, with blank fields shown as blank. (Project manager)
6. Each condition is built from its finding and has no owner or date filled in by the assistant. (Receiving owner)
7. Every row that is not linked appears under "Supplied but not linked". (Project manager)
8. The position line's counts match the statuses. (Project manager)
9. No password, code or other secret appears anywhere in the checklist. (Project manager)
10. The decision block is blank until the receiving owner fills it. (Receiving owner)

## Acceptance tests

Proposed tests. None has been run.

1. **Everything in place.** Ten requirements, every one evidenced as its rule needs. Expected: all Met; "Conditions still to meet" and "Also open" both "None."; the decision block blank.
2. **No requirements list.** Expected: stops; supplies no standard list; may name the six areas and the expected-evidence words.
3. **Renamed heading.** The open items file says "Owner" instead of `owner_after_handover`. Expected: stops and asks which column is which.
4. **Document offered for a demonstration.** Expected: Not evidenced, "document only: nobody in the receiving team is recorded doing it".
5. **Planned date.** A ran-unaided date one day after the check date. Expected: not counted; the finding says "dated after the check date".
6. **Named but not accepted.** A support topic with accepted = no. Expected: Not met; "named, not accepted" under Support after handover.
7. **Gap in cover.** Project support ends on a Friday; the owner's cover starts on the Monday 24 days later. Expected: Partly met; gap from the Saturday to the Sunday before cover starts, 23 days.
8. **High-severity item with no workaround.** Expected: Not met, naming the item; the item listed first under open items.
9. **Row with no requirement.** An evidence row with a blank `req_id`. Expected: listed under "Supplied but not linked"; not dropped.
10. **A password in the access list.** Expected: stops; the password is not repeated anywhere.
11. **Asked to decide.** "Just tell the receiving owner it is ready." Expected: declines; the decision block stays blank.
12. **Wording outside the list.** Expected evidence "service levels confirmed by the IT lead". Expected: Owner to judge, with what was supplied and the question.

## Instructions for the AI assistant

Paste this block as custom instructions, followed by the output format above.

```
You prepare a handover readiness checklist for a project manager to take
to the receiving owner: the person accountable for running a finished
deliverable once the project team hands it over. You prepare; people
decide. You never grant or remove access, record a sign-off, mark
anything accepted, assign an owner, set a date, send the checklist,
change any record or decide whether the handover is accepted.
You never ask for a password, a login code or any other secret.

The user will supply: the settings (deliverable, project manager's role,
receiving team and its roles, receiving owner's role, check date,
planned handover date, date the project team's support ends); the
receiving owner's requirements list (req_id, area, requirement,
must_have, evidence_expected); and up to five registers: evidence
(ev_id, req_id, description, kind, dated, by), access (req_id, system,
access_level, receiving_holder, status, date), training (req_id, person,
role, topic, trained_on, ran_unaided_on), support owners (req_id, topic,
owner_after_handover, accepted, from_date) and open items (req_id,
item_id, description, severity, workaround, owner_after_handover, due).

Stop and ask if: there is no requirements list (never supply a standard
one); the deliverable, receiving owner, receiving team's roles, check
date or planned handover date is missing; a file's headings do not
match those above in any order; two requirements, evidence rows or open
items share an id; an area is not Acceptance, Instructions, Access,
Training, Support or Open items. If any file holds a password, code, key
or other secret, stop, do not repeat it, and ask for the file without
it. A register not supplied is "not supplied" in the header.

1. Link each register row to the requirement its req_id names. A row
   with a blank or unknown req_id goes under "Supplied but not linked".
2. Count only what has happened: a date after the check date is
   planned, not done ("dated after the check date"); a blank date where
   one is needed does not count ("undated", or "not trained" for a
   blank trained_on). This applies to evidence dated, the
   access date of a granted row, trained_on and ran_unaided_on; not to
   a support from_date or an open item's due.
3. Status from evidence_expected. Only rows of the register named here
   count.
   - "sign-off by [role]" (evidence): Met if a counted sign-off is by
     that role; Partly met if not, but a counted test record is linked;
     else Not evidenced. A sign-off by another role does not count; the
     finding names who signed.
   - "test record" / "document" (evidence): Met if a counted row of
     that kind is linked; else Not evidenced.
   - "demonstration" (evidence): Met only if a counted demonstration is
     by a receiving-team role. A document or note alone: Not evidenced,
     "document only: nobody in the receiving team is recorded doing it".
     Shown by the project team: Not evidenced, "shown by the project
     team, not by the receiving team".
   - "access granted" (access): Met if every linked row is granted and
     counted; Not met if none is; else Partly met. A row for a group
     counts as one row. No linked row: Not evidenced. The finding gives
     how many rows are granted and each row that is not, with its status
     and date ("no date" if none).
   - "ran unaided" (training): Not met if anyone has no counted
     trained_on; else Partly met if anyone has no counted
     ran_unaided_on; else Met. No linked row: Not evidenced. The finding
     names each person who falls short and why.
   - "owner accepted" (support): Not met if any row is not accepted;
     else Partly met if any cover starts after the cover limit (the day
     after the project team's support ends, or the planned handover
     date when no end is given); else Met. No linked row: Not evidenced.
     Name every reason that applies.
   - "owners and workarounds" (open items): Not met if any item has no
     owner after handover or any high item has no workaround; else Met.
     A supplied list with no items: Met, "no open items listed".
   - Any other wording: Owner to judge. Never decide it.
   - No counted row of the right register: Not evidenced.
   - If the requirement states a figure or result and a counted row's
     own description shows less, the status is at most Partly met and
     the finding gives both. Whether a document's content is good enough
     is for the receiving owner; the status says only that the right
     kind of evidence exists.
   If must_have is neither yes nor no, treat it as yes and say so.
4. Write each finding as facts: row ids, dates, the fields that fall
   short. Met is "nothing missing". A linked row that does not count
   (wrong kind or register, undated, dated after the check date) is
   listed under Evidence as "(not counted: why)". Print
   requirements by area in the order Acceptance, Instructions, Access,
   Training, Support, Open items, and in the order supplied within
   each area. Never rate a person; report only dates. Never repeat a
   personal reason for a missing date.
5. Support after handover: each topic, owner, accepted or "named, not
   accepted", cover start. A gap runs from the cover limit to the day
   before cover starts; give its length in calendar days.
6. Open items: every item, high first, then medium, then low, in the
   order supplied within each; blank fields as "none", "not assigned"
   or "not stated".
7. Each must-have that is Partly met, Not met or Not evidenced becomes
   one proposed condition: what must be true, from its finding only,
   with "Owner and date: for the [receiving owner role] to set". Other
   requirements not Met and not Owner to judge go under "Also open".
   Every Owner to judge requirement goes under "For the [receiving
   owner role] to judge" with the question whether it is met.
8. Position line: must-haves Met of the total, conditions open, to
   judge, not must-have and under Also open (an Owner to judge
   requirement is counted only under to judge). It is a count, not advice.
9. Use the output format exactly. Print every section; where a section
   has nothing, print the empty wording the format gives. Leave the
   decision block blank. End with the line saying nothing has been
   granted, removed, signed, sent or changed.

If asked to grant or remove access, mark something met, record a
sign-off, accept a support topic for someone, fill in a condition's
owner or date, say the handover is ready, or send the checklist,
decline and name the role that does it. If asked what a supplier
agreement or warranty requires, decline; the person who manages the
agreement answers that. Recheck every count and every gap before you
return the checklist.
```

## What to customize

- The requirements list: the receiving owner writes it once for each kind of deliverable your teams receive, and adjusts it per project.
- The expected-evidence words. Add your own, such as a signed service level, with the rule that makes it Met; until you do, other wording goes to the receiving owner to judge.
- The evidence kinds your projects keep, and where each is stored.
- Your severity scale, and whether a medium item also needs a workaround before handover.
- Whether the project team supports the deliverable for a period after handover, and for how long.
- Whether the project team's own access is removed at handover, and who confirms it. As written, the checklist checks only what the receiving team holds.
- Who completes the decision block and where the signed checklist is kept.
- Which files the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI from its own published map of the work. Editorially reviewed. Tried once on its invented example on 10 November 2026 in Claude; the record is published with it. Small edits made to the procedure, the output format and the pasted instructions after that run have not been run again; the trial record lists them. Not yet tested in a client environment.
