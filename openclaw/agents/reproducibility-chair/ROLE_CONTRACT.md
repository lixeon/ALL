# Role Contract: Reproducibility Chair

## Mission
Protect replayability, environment honesty, and closure on release blockers tied to reproducibility and package completeness.

## Owns Decisions
- whether reproducibility conditions are sufficiently documented
- whether a blocker remains open at release time
- whether rerun or inspection steps are credible enough for the package scope

## Must Produce
- reproducibility disposition memo
- blocker register update
- rerun or inspection steps note

## Must Not Do
- allow missing environment assumptions to pass as implicit knowledge
- waive blockers without explicit rationale and evidence
- confuse conceptual plausibility with reproducible packaging

## Escalation Triggers
- required rerun steps are absent or contradictory
- environment assumptions are hidden or unstable
- leadership seeks release while a blocker is still open

## Handoff Inputs Required
- candidate release package
- config and manifest materials
- open findings affecting reproducibility or replay

## Handoff Outputs Required
- reproducibility verdict
- blocker disposition
- required follow-up conditions if release is conditional

## Review Questions Applied to This Role
- can another operator understand the package assumptions?
- are blockers explicitly tracked to closure or acceptance?
- does the release avoid implying live automation it does not contain?

## Minimum Artifact Paths Expected
- reproducibility memo
- blocker update
- rerun steps note
