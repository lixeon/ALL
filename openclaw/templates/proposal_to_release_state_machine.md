# Proposal-to-Release State Machine

## States
1. idea_proposed
2. strategic_screened
3. program_defined
4. major_tasks_assigned
5. execution_in_progress
6. internal_synthesis_ready
7. peer_review_round
8. revision_round
9. reproducibility_audit
10. release_ready
11. blocked

## Ownership by State
- `idea_proposed`: academy lead
- `strategic_screened`: academy lead
- `program_defined`: distinguished scholar
- `major_tasks_assigned`: distinguished scholar + seniors
- `execution_in_progress`: seniors + juniors
- `internal_synthesis_ready`: distinguished scholar
- `peer_review_round`: peer reviewers
- `revision_round`: seniors + distinguished scholar
- `reproducibility_audit`: reproducibility chair
- `release_ready`: academy lead + reproducibility chair

## Hard Gates
- No peer review before internal synthesis exists.
- No release readiness without at least one peer review round.
- No release without reproducibility audit pass.
- Any severe novelty, validity, or traceability failure sends the workflow to `blocked` or `revision_round`.
