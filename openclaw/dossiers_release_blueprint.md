# Release Dossier Blueprint

## Purpose
This blueprint defines the minimum dossier that should accompany an OpenClaw academic team release.
It is designed for external inspection, internal replay, and reproducibility review.

## Dossier Structure

### 1. Executive Abstract
- release id
- one-paragraph thesis
- claimed contributions
- current confidence level

### 2. Research Question Register
- primary question
- secondary questions
- excluded questions
- novelty boundary statement

### 3. Team Contribution Ledger
For each role, capture:
- role name
- major deliverables produced
- critical decisions made
- unresolved concerns handed forward

### 4. Evidence and Artifact Index
For each key artifact, capture:
- artifact id
- filesystem path
- producing role
- creation stage
- validation status
- notes for re-use or replay

### 5. Review Findings Register
Track every meaningful reviewer finding with:
- finding id
- reviewer
- severity
- concern summary
- required action
- closure status
- closure evidence path

### 6. Reproducibility Disposition
- environment assumptions
- config package used
- required rerun steps
- missing dependencies or caveats
- chair verdict: pass, conditional, or fail

### 7. Claim-to-Evidence Matrix
Each major claim should map to:
- supporting artifacts
- supporting analyses
- known limitations
- reviewer pressure applied

### 8. Release Decision Memo
- academy lead decision
- scholar recommendation
- reasons for release or hold
- follow-up work for next version

## Minimum Acceptance Rule
If the dossier cannot explain what was built, why it should be believed, and how it can be checked, the release is not ready.

## Example Skeleton

```text
release_id: V8
thesis: OpenClaw academic teams benefit from explicit governance and release dossiers.
confidence: medium

finding_id: PR1-02
severity: high
concern: Evaluation claim exceeds demonstrated evidence.
required_action: Narrow contribution language and add artifact-backed limitation note.
closure_status: fixed
closure_evidence_path: /openclaw/dossiers/examples/V8_release_dossier_example.md
```

## OpenClaw Usage Note
The dossier should be updated incrementally rather than authored only at the end.
That makes reviewer closure, artifact indexing, and release decisions easier to audit.
