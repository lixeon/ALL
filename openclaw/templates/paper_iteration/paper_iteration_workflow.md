# Paper Iteration Workflow (Reject → Revision → Resubmit)

## Purpose
Simulate realistic academic paper writing with multi-agent co-authoring and reviewer-driven iteration.

## Core Artifacts
- manuscript drafts: `manuscript/draft_v*.md` and/or `manuscript/draft_v*.tex`
- response letters: `reviews/response_v*.md`
- decision records: `reviews/decision_v*.json`
- change logs: `manuscript/change_log.md`

## Roles
- `paper-writer`: manuscript owner, integrates content and revisions
- `latex-editor`: format/compile owner, submission packaging
- `senior-researcher-*`: technical section owners, evidence owners
- `junior-researcher-*`: experiment + reproduction notes, table/figure prep
- `peer-reviewer-*`: external-style reviewers, can reject and demand revision
- `distinguished-scholar`: synthesis editor, resolves conflicts
- `academy-lead`: strategic accept/reject of direction, final endorsement
- `reproducibility-chair`: blocks release if claims are not traceable

## Workflow Stages
### Stage 0: Inputs Ready
- evidence artifacts exist (benchmarks, runs, logs)
- claim register exists and is minimally filled

### Stage 1: Draft v1
- paper-writer produces `draft_v1.md`
- seniors provide method/results content
- juniors provide tables/plots + provenance

### Stage 2: Internal Lab Review
- distinguished-scholar requests structured critique from seniors
- reproducibility-chair checks traceability for the top claims

### Stage 3: External Peer Review Simulation
- peer-reviewer-1 issues novelty/positioning review
- peer-reviewer-2 issues validity/reproducibility review
- each review ends with: {ACCEPT | MINOR | MAJOR | REJECT}

### Stage 4: Decision + Revision Plan
- paper-writer compiles all comments into a revision checklist
- seniors accept assigned revisions
- academy-lead may block the line if significance is not emerging

### Stage 5: Revision Cycle
- draft_v(k+1) produced with change log
- response letter updated point-by-point
- reproducibility-chair re-audits changed claims

### Stage 6: Exit Gate
Exit only when:
- peer reviewers are no longer in REJECT/MAJOR mode
- reproducibility-chair passes traceability + rerun readiness
- academy-lead endorses direction

## Failure Handling
- If REJECT persists for 2+ cycles: require thesis reframing by distinguished-scholar
- If traceability fails: reproducibility-chair blocks release until fixed
