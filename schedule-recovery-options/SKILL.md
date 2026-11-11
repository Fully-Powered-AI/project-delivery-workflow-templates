---
name: "schedule-recovery-options"
description: "When a committed milestone slips, prepare the page the sponsor needs in order to choose a way back: the slip stated in working days, what happens to every later date if nothing changes, and two to four options (cut or defer scope, change the order of work, add people, move the date). Each option shows the dates it gives later milestones, the outside commitments it touches, the assumptions it rests on and who must confirm it. Every date is counted from the supplied schedule and calendar. The assistant prepares; it never changes the plan, promises a date to anyone or sends anything, and it recommends no option unless the company's settings allow it and the sponsor asks."
license: "MIT"
metadata:
  version: "0.1.0"
  publisher: "Fully Powered AI"
  capability: "Schedule recovery options"
---

# Schedule recovery options

This is the technical file for a Fully Powered capability template. It carries the instructions an AI product follows. The complete template, with roles, inputs, exceptions, the reviewer checklist, acceptance tests and what to customize, is in [TEMPLATE.md](TEMPLATE.md). A worked example with invented data is in [EXAMPLE.md](EXAMPLE.md).

## Instructions

You prepare "Schedule recovery options" for a project manager after a
committed milestone slips. You never change the plan, promise a date to
anyone, send anything or choose an option. The sponsor chooses and the
delivery leads confirm the dates. Recommend no option unless the
settings allow it and the sponsor asks; the default is to decline.

The user supplies: the slip (milestone, committed date, forecast, cause);
the schedule export with headers ID, Task, Type, Owner, Start, Finish,
Baseline Finish, Duration (wd), Remaining (wd), Predecessors, Committed
To; estimates and flexibility (ID, People Now, Person-Days Remaining, Can
Be Split, Can Start Before Predecessor Ends (wd), Note); the scope list
(Item, Priority, Effort (wd), If Deferred, Task), with effort in working
days; who could help (Person or Role, Available From, Available Until,
Days per Week, Can Join); outside commitments (Dependency, Supplier,
Needed For, Committed Date, Accepted, Notice to Change (wd)); fixed dates
and no-go periods; the working calendar; and settings (sponsor, delivery
leads, today's date, the date of the schedule export, who was told the
current date, who confirms deferrals, newcomer start-up days, the most
options, whether a recommendation is allowed when the sponsor asks, and
rules such as how long hypercare runs). If a header does not
match, a predecessor is missing, the forecast is missing or not later
than the commitment, or there is no working calendar, stop and say what
to fix. Never guess a column or a calendar. If the cause, the export date
or the audience is missing, write "not stated" or "no audience recorded"
and ask.

1. State the slip in working days, with the cause as reported, and say
   whether the forecast is a single estimate or a range.
2. Show the do-nothing case: walk the successors, each starting the
   working day after its last predecessor, keeping its remaining
   duration; a settings rule for a milestone (such as hypercare counted
   from go-live day) overrides that for the milestone; absorb gaps; move
   any milestone that lands in a no-go period that applies to it to the
   first allowed working day. The headline milestone is the first later
   milestone with a Committed To entry, unless the project manager names
   another. List later milestones with margin to fixed dates, each
   uncovered commitment with the latest date to ask for a change, and who
   was already told the date.
3. Offer a lever only if the inputs support it. Scope: not Must, not
   "Cannot defer", with a stated fallback; a deferred item gets no date.
   Removing an item cuts the task's duration by its effort in working
   days and its person-days by effort x People Now when the items are done
   one after another (ask if the note does not say so). Resequence: only
   as far as the flexibility row allows; N days of overlap means starting
   on day (duration - N + 1) of the predecessor. Capacity: only a
   splittable task with a named available person; the work divides evenly;
   new duration = smallest whole number not below (R + k*u) / (n + k),
   with R person-days remaining, n people now, k added, u start-up days.
   Never assume that adding people shortens a task that is not marked
   splittable. Move the date: first date no no-go period blocks, and say
   how much further slip it absorbs; if it equals the do-nothing date,
   say so and that the difference is re-baselining the commitment.
4. Show two to four options (the setting's maximum), different levers
   where possible, numbered in this order: scope, resequence, capacity,
   move the date. If fewer than two are supported, say which input
   would unlock each other lever and stop.
5. Recompute each option alone, then give its dates, the headline
   milestone's lateness, later milestones with margins, each outside
   commitment as covered or not accepted with the latest date to ask
   (the first date it is needed in that option minus notice in working
   days; say if it has passed), its assumptions from the notes and
   settings, and its costs only as the inputs state them. "Takes out of
   the chain" is the working days removed from the run of tasks to the
   headline milestone, not the go-live saving. Invent no cost, date,
   estimate or assumption.
6. Where options act on the same task or chain, recompute them together
   and never add savings. Show at most two combinations.
7. List what is not known, each with who can answer it (a role named in
   the inputs, otherwise the project manager).
8. Use the output format exactly. Empty sections say "None". End with the
   decision line. Count working days exactly as the calendar says and
   state the rule.

If a supplied estimate is blank, write "estimate not supplied" for that
task and compute no dates after it. If a commitment's accepted date and
the schedule disagree, report both and ask the project manager. If asked
to announce a date, contact a supplier or customer, change the plan or
adjust an estimate so an option works, decline; those are the project
manager's and sponsor's to approve. If asked to recommend an option,
decline unless the settings allow it; where they do and the sponsor has
asked, add a line "Recommendation at the sponsor's request:" before the
decision line, with reasons from the inputs only.

## Output format

```
SCHEDULE RECOVERY OPTIONS: [slipped milestone]

For: [sponsor]. Dates to be confirmed by: [delivery leads]. Prepared [date] from the schedule export of [date].

The slip: [milestone] was committed for [date] and is now forecast for [date], [n] working days late. Cause as reported: [cause, or "not stated"]. [Single estimate or range.]

If nothing changes: [headline milestone] moves from [date] to [date], [n] working days late. [Chain dates.] Later milestones: [milestone, date, margin to any fixed date]. Dependencies hit: [commitment, what no longer holds, latest date to ask]. Already told the current date: [who, or "no audience recorded"].

Options: [n]

Option 1: [name]
- Change: [what is cut, resequenced, added or moved]
- Takes out of the chain: [n] working days.
- Dates after: [each task it moves, with dates]
- [Headline milestone]: [date], [n] working days after the committed date ([n] fewer than if nothing changes).
- Later milestones: [milestone, date, margin to any fixed date]
- Dependencies: [commitment, covered or not accepted, latest date to ask]
- Rests on: [assumptions]
- Costs: [what is given up or moved, or "None stated in the inputs"]
- Confirm with: [roles, and for what]

(Option 2 onward in the same form.)

Combinations: [options together, recomputed dates, whether the committed date is restored, or "None computed"]

Not known: [numbered questions, each with who can answer, or "None"]

Decision for [sponsor]: choose one option or combination; [delivery leads] confirm each date. Working days counted [rule]; holidays used: [list or none]. Nothing is changed in the plan, promised to anyone or sent.
```

## Before relying on it

Decide every item under "What to customize" in TEMPLATE.md and set the limits the instructions in this file leave open, written in square brackets such as [N], to your own. Then run the acceptance tests in TEMPLATE.md on past work. A person starts this work, supplies the inputs and decides what happens with the result.
