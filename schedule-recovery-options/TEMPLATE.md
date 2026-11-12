# Schedule recovery options

Workflow template, version 0.1.0.

## Purpose

When a committed milestone slips, prepare the page the sponsor needs in order to choose a way back: the slip stated in working days, what happens to every later date if nothing changes, and two to four options (cut or defer scope, change the order of work, add people, move the date). Each option shows the dates it gives later milestones, the outside commitments it touches, the assumptions it rests on and who must confirm it. Every date is counted from the supplied schedule and calendar. The assistant prepares; it never changes the plan, promises a date to anyone or sends anything, and it recommends no option unless the company's settings allow it and the sponsor asks.

## When to use it and when not to

Use it as soon as a milestone the project has committed to is forecast to miss its date, and before the sponsor is asked to react. It also suits a slip that has already happened if no choice has been made.

Do not use it to report general progress (use Project status report), to look for how a plan could fail before approval (use Premortem before a decision), or to record the sponsor's choice afterwards (use Decision log). Do not use it when the forecast is earlier than the commitment, when the schedule has no dependencies recorded, or to negotiate with a supplier or customer, which is a person's work.

## Roles

- **Runs it:** the project manager.
- **Chooses the option:** the sponsor.
- **Confirms feasible dates and assumptions:** the delivery leads who own the tasks, and any person the inputs name as confirming a deferral or a release of people.
- **Owns each outside commitment and any request to change it:** the role named on the commitment.
- **Records the decision:** the project manager.

## Inputs

1. **The slip:** the milestone ID, the date committed, the new forecast, and the cause in the words of the person reporting it. If the forecast is missing, stop. If the cause is missing, write "not stated" and ask for it.
2. **The schedule export,** one row per task or milestone, with these default headers: `ID, Task, Type, Owner, Start, Finish, Baseline Finish, Duration (wd), Remaining (wd), Predecessors, Committed To`. If a header does not match, stop and ask which supplied column to use for it. Do not guess.
3. **Estimates and flexibility** from the delivery leads, default headers: `ID, People Now, Person-Days Remaining, Can Be Split, Can Start Before Predecessor Ends (wd), Note`. If missing, no capacity or resequencing option is offered, and the page says why.
4. **The scope list,** default headers: `Item, Priority, Effort (wd), If Deferred, Task`. Effort is in working days of the named task's current duration. Priorities are the company's labels; "Must" and any item marked "Cannot defer" are never offered for deferral. If missing, no scope option is offered.
5. **Who could help,** default headers: `Person or Role, Available From, Available Until, Days per Week, Can Join`. If missing, no capacity option is offered.
6. **Outside commitments,** default headers: `Dependency, Supplier, Needed For, Committed Date, Accepted, Notice to Change (wd)`. If missing, say that dependencies were not checked.
7. **Fixed dates and no-go periods** (for example a licence end or a close week), each with whether it can move. If missing, say none were supplied.
8. **The working calendar:** working days, holidays, freeze periods. If missing, stop and ask; do not assume.
9. **Settings:** sponsor, delivery leads, today's date, the date of the schedule export, who has already been told the current date of the headline milestone and which date they were told, who confirms a deferral that touches their area (for example a team whose report or process the fallback relies on), the number of working days a newcomer needs before they help (default 3), the most options to show (default 4), whether the assistant may give a recommendation when the sponsor asks (default: no, it declines), and any rule such as how long hypercare runs.

## The procedure

1. **Check the inputs.** Match every header. Check every predecessor ID exists and the chain from the slipped milestone has no loop. If anything fails, stop and list what to fix.
2. **State the slip.** Count the working days from the committed date to the forecast date. Give the cause in the reporter's words. Say whether the forecast is a single estimate or a range.
3. **Show what happens if nothing changes.** Move the slipped milestone to its forecast. Walk its successors in order: a task starts on the working day after its last predecessor finishes and keeps its remaining duration; a task with several predecessors waits for the latest. A rule in the settings for a particular milestone (for example hypercare "counted from go-live day") overrides the successor rule for that milestone. A task that already finished earlier than a successor needs it absorbs the slip up to that gap. If a milestone then lands inside a no-go period that applies to it, move it to the first allowed working day. The headline milestone is the first later milestone with an entry under Committed To, unless the project manager names another. Count its lateness in working days. List every later milestone with its new date, its margin to any fixed date (the working days after it, up to and including the fixed date), each outside commitment whose accepted date no longer covers the new date with the latest date to ask for a change (as in step 7), and who was already told the current date, from the settings.
4. **Find the levers the inputs support.** Offer a lever only if the inputs make it real.
   - **Cut or defer scope:** only an item that is not "Must", is not marked "Cannot defer" and has a stated fallback. Remove its effort from its task: the task's duration falls by the item's effort in working days, and its person-days fall by the effort multiplied by the task's People Now when the items are done one after another. If the task's note does not say the items run one after another, ask before converting. A deferred item gets no date; say it needs its own decision.
   - **Resequence:** only a task whose flexibility row allows an earlier start. It may start the stated number of working days before its predecessor ends, never more. N working days of overlap means starting on day (duration − N + 1) of the predecessor: 3 days of overlap on a 5-day predecessor starts on its third day.
   - **Add capacity:** only a task marked as splittable, with a named person available over the dates. With R person-days remaining, n people now, k added and a newcomer start-up of u working days, the new duration is the smallest whole number of days not below (R + k × u) / (n + k). If the task is not marked splittable, adding people is not assumed to shorten it; say so. The work is taken to divide evenly across the people.
   - **Move the date:** keep scope, order and people, and set the headline milestone to the first date the work finishes that no no-go period blocks. State how many working days of further slip the new date absorbs. If the new date equals the do-nothing date, say so: the dates are the same, and the difference is that the commitment is re-baselined to the new date.
5. **Pick two to four options,** up to the setting, preferring different levers. Number them in this order, leaving out any lever not offered: cut or defer scope, resequence, add capacity, move the date. If fewer than two are supported, say so, list which input would unlock each lever that was not offered, and stop there.
6. **Recompute each option on its own.** Rebuild the chain with only that change. "Takes out of the chain" is the working days removed from the run of tasks between the slipped milestone and the headline milestone (after overlaps); it is not the go-live lateness saving, which can be larger when the option also avoids a no-go period. Give the new dates of every task it moves, the headline milestone's date, its lateness in working days against the commitment, and how many fewer working days late than if nothing changes.
7. **Knock-on effects.** For each option, list every later milestone with its date and margin to any fixed date; list each outside commitment as covered, or not accepted for the new date. For each uncovered commitment, give the latest date to ask for a change: the first date the commitment is needed in the option's schedule (for support on go-live, the go-live date) minus the commitment's notice in working days. If that date has passed, say so. Name any internal person whose release the option needs.
8. **Assumptions and costs.** For each option list what it rests on, taken from the notes and settings, plus the standard ones: the slipped milestone finishes on its forecast; the estimates hold; for added capacity, the work divides evenly across the people. An assumption that is in neither the notes nor the settings is a question under step 10, not an assumption. List what the option gives up or moves, only as the inputs state it. Invent no cost.
9. **Combinations.** Where two options act on the same task or the same chain, recompute them together; never add their savings. Show up to two combinations worth the sponsor's time, each with its dates, and say whether the committed date is restored.
10. **Not known.** List every question that changes a date or an assumption, each with who can answer it. Take the answerer from a role named in the inputs; if none is named, it is the project manager.
11. **Close.** Name the working-day counting rule and holidays used. Return the draft to the project manager only.

## Exceptions and stop conditions

- **A header does not match, or a predecessor ID is missing:** stop; list the problem.
- **No working calendar:** stop; ask.
- **The forecast is not later than the commitment:** stop; there is no slip.
- **The slipped milestone has no successors:** say so; the only effect is its own lateness.
- **A supplied estimate is blank:** write "estimate not supplied" for that task and do not compute dates after it.
- **A commitment's accepted date and the schedule disagree:** report both and ask the project manager.
- **Asked to recommend an option when the settings do not allow it, or to promise a date to a customer or supplier, change the plan, or write the message announcing the new date:** decline; the sponsor chooses and the project manager decides what is said and to whom. Where the settings allow a recommendation and the sponsor asks, the instruction block says how it is given.
- **Asked to adjust an estimate so an option works:** decline.

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

## Reviewer checklist

1. The number of working days late is correct against the supplied calendar. (Project manager)
2. If-nothing-changes dates follow the predecessors, durations and no-go periods. (Project manager)
3. Every option changes only what the inputs allow, and its dates were recomputed. (Delivery leads)
4. No combination adds the savings of options that act on the same task. (Project manager)
5. Every outside commitment is marked covered or not accepted, with the latest date to ask. (Delivery lead who owns it)
6. Every assumption is stated and every cost comes from the inputs. (Delivery leads)
7. Nothing recommends an option, promises a date or announces one. (Project manager)
8. Every empty section says "None". (Project manager)

## Acceptance tests

Proposed tests. None has been run. They use the worked example's inputs.

1. **Normal slip.** M1 committed Fri 18 Jun, forecast Fri 2 Jul. Expected: 10 working days late; if nothing changes, go-live Mon 9 Aug (15 working days late) because Mon 2 Aug falls in the Finance close.
2. **Scope option.** Reports module deferred. Expected: UAT 7 working days, go-live Wed 28 Jul, Vendor B booking needed by Wed 14 Jul, and a note that the deferred module has no date.
3. **Capacity formula.** One tester added to a 20 person-day task with 2 people and a 3-day start-up. Expected: 8 working days, saving 2.
4. **Overlap.** Preparation allowed to start 3 working days before training ends. Expected: starts the third day of training, and no more.
5. **Combinations.** Defer Reports (Option 1), the overlap (Option 2) and the added tester (Option 3) together. Expected: Reports' 3 working days on 2 people are 6 person-days, so 14 remain and UAT takes 6 working days; 7 working days taken out of the chain, not 8; go-live Thu 22 Jul.
6. **Not splittable.** The flexibility row says the task cannot be split. Expected: no capacity option, with a line that adding people is not assumed to shorten it.
7. **Header mismatch.** The schedule's "Finish" column is called "End date". Expected: stops and asks.
8. **Asked to recommend.** The settings do not allow a recommendation. Expected: declines; lists the options with facts.
9. **Uncovered commitment with a passed deadline.** The latest date to ask is before today. Expected: says it has passed.
10. **Move the date equals doing nothing.** In the worked example the no-go period has already moved go-live to Mon 9 Aug. Expected: Option 4 says its dates equal the do-nothing dates and that it re-baselines the commitment.
11. **Settings rule for a milestone.** Hypercare is counted from go-live day. Expected: hypercare ends Fri 20 Aug when go-live is Mon 9 Aug, not the working day after go-live.
12. **Missing export date or audience.** No schedule export date or list of who was told is supplied. Expected: the page says "not stated" or "no audience recorded" and asks, and does not guess.

## Instructions for the AI assistant

```
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
```

## What to customize

- The headers of your schedule export, and the priority labels in your scope list.
- Your working calendar, holidays and freeze periods.
- The start-up days a newcomer needs and which kinds of task your people accept can be split.
- The notice each supplier or team needs for a change.
- The most options shown, and whether the assistant may recommend when the sponsor asks (the default is that it declines).
- What counts as the headline milestone, and any fixed dates always checked, such as a licence end.
- Who confirms deferrals and releases of people, besides the delivery leads.
- Which exports the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI from its own published map of the work. Not yet tested in a client environment.
- 10 November 2026, revised after review: effort in working days converted to person-days, the order of options fixed, settings that override the successor rule, today's date, the export date and the list of who was told added to the inputs, "takes out of the chain" and the overlap and notice rules defined.
