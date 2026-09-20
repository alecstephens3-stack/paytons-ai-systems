# Progress Records

Use these records when repeated work needs evidence over time. Keep them with the decision they support. Use only the sections that can change a decision, and preserve every original forecast, stop rule, trigger, and metric definition.

## Forecast and actual

- **Record ID:** [stable label]
- **Linked decision:** [decision log entry]
- **Forecast class:** [stable label for sufficiently similar forecasts]
- **Forecast date:** [YYYY-MM-DD]
- **Predicted event or value:** [event, value, or range]
- **Probability or confidence:** [number with a basis, or a plain-language confidence]
- **Resolution date or condition:** [when the forecast becomes answerable]
- **Resolution source:** [evidence that will settle it]
- **Actual result:** [append after resolution]
- **Resolved on:** [YYYY-MM-DD]
- **Error or miss:** [difference between predicted and actual, using the same units]

Compare only forecasts with the same class, units, and resolution rule. State the number of resolved forecasts and any limits before describing a bias or applying a correction. Do not turn unrelated examples into one calibration score.

## Experiment

- **Record ID:** [stable label]
- **Linked decision:** [decision log entry]
- **Hypothesis:** [change and expected result]
- **Baseline and source:** [current result, date, population, and window]
- **Test action:** [one bounded intervention]
- **Test window:** [start and end condition]
- **Cost or effort budget:** [maximum acceptable spend, time, or effort]
- **Outcome measure:** [definition and source]
- **Success condition:** [result that would support the hypothesis]
- **Guardrail:** [result that must not deteriorate]
- **Stop rule:** [link to a criterion written in KILL CRITERIA.md before the test]
- **Observed result:** [append evidence after the test]
- **Decision:** [continue, change, stop, or collect one named observation]

## Trigger-action check

- **Record ID:** [stable label]
- **Cue:** [observable event]
- **Action:** [feasible response]
- **Owner:** [person or role]
- **Rehearsal result:** [date and what happened in a dry run]
- **Check window:** [when the cue could occur]
- **Did the cue occur?:** [yes, no, or unknown, with evidence]
- **Did the action occur?:** [yes, no, or unknown, with evidence]
- **Failure diagnosis:** [cue, action size, missing input, capacity, conflict, or changed goal]
- **Next change:** [keep, revise, remove, or collect one named observation]

Do not assume a missed action proves the cue failed. Check whether the cue happened and whether the action was possible.

## Metric and countermetric

- **Record ID:** [stable label]
- **Linked decision:** [decision log entry]
- **Intended real-world outcome:** [change for the user, work, or business]
- **Outcome metric and proxy limit:** [name, definition, and what it may miss]
- **Countermetric:** [quality, risk, cost, or other protected result]
- **Ground-truth check:** [direct inspection or qualitative feedback]
- **Source, population, and window:** [keep these stable or record the change]
- **Baseline:** [value and date]
- **Latest result:** [value and date]
- **Interpretation:** [what changed, what did not, and data limits]
- **Decision:** [action this evidence changes, or no change]

An improved outcome metric is not a win when the countermetric shows unacceptable harm.

## Due-record review

| Record ID | Type | Due date or observable trigger | Owner | Evidence available | Status | Linked review |
|---|---|---|---|---|---|---|
| [ID] | [forecast, experiment, trigger, or metric] | [condition] | [owner] | [source, missing, or delayed] | [open, resolved, overdue, or closed] | [AFTER ACTION REVIEW.md entry or none] |

At an existing authorized review:

1. Find records whose date or trigger has arrived.
2. Close a record only with the stated resolution evidence.
3. Mark missing or delayed evidence plainly instead of inventing a result.
4. Link a material result to `AFTER ACTION REVIEW.md` and preserve the original prediction, stop rule, and metric definition.
5. Assign the next owner and condition, or close the record with no further review.

This review does not create a calendar event, reminder, monitor, or automation.
