# Release Assembly Workflow

## Purpose
Define how the OpenClaw academic team converts scattered role outputs into one inspectable release package.

## Stage 1: Freeze Candidate Scope
- `distinguished-scholar` names the candidate thesis package.
- `academy-lead` confirms the scope is strategically coherent.
- seniors list the exact artifacts proposed for inclusion.

## Stage 2: Build Registers
- each senior submits artifact paths and claim mappings.
- peer reviewers submit finding ids, severities, and closure tests.
- `reproducibility-chair` opens a run ledger and a finding register for the candidate.

## Stage 3: Validate Package Integrity
- verify required files against the package manifest
- verify every major claim has at least one linked artifact path
- verify every open high-severity finding is either fixed or blocks release
- verify rerun notes exist for any evidence that materially affects conclusions

## Stage 4: Compose Release Dossier
- populate executive abstract
- populate contribution ledger by role
- attach claim-to-evidence matrix
- attach finding closure status
- record final reproducibility disposition

## Stage 5: Decision and Snapshot
- `academy-lead` records release or hold decision
- `reproducibility-chair` records pass, conditional, or fail
- snapshot the package under a new versioned release directory
- update release notes and index files without changing prior releases

## Failure Conditions
Stop assembly if any of the following remain true:
- major claim has no path-backed evidence
- reviewer finding closure cannot be audited
- manifest and package contents disagree
- release notes imply stronger automation than the package really supports
