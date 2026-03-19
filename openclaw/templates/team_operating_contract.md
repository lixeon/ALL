# OpenClaw Academic Team Operating Contract

## Purpose
This document defines the operating contract that binds the 9-agent academic team into a predictable OpenClaw execution system.
It adds explicit governance, escalation, artifact discipline, and release controls that were only implicit in V7.

## Operating Principles
1. Every claim must have an owner.
2. Every artifact must have a path.
3. Every delegation must have a return condition.
4. Every review must be adversarial but evidence-based.
5. Every release must preserve a complete reconstruction trail.

## Team Authority Map

### Academy Lead
- owns research program legitimacy and final release authorization
- can stop, redirect, or narrow scope when claims exceed evidence
- arbitrates deadlocks that remain unresolved after reviewer discussion

### Distinguished Scholar
- owns intellectual synthesis across all workstreams
- translates leadership direction into researchable packages
- decides whether work products are coherent enough for review

### Senior Researchers
- own methodology, experiment design, and synthesis quality within assigned tracks
- may delegate execution to juniors, but retain accountability for rigor
- must return with explicit assumptions, risks, and unresolved issues

### Junior Researchers
- own execution throughput, artifact preparation, and evidence assembly
- must not silently reinterpret goals when tasks become ambiguous
- must escalate missing data, broken assumptions, or blocked tooling quickly

### Peer Reviewers
- own adversarial review from novelty, validity, evaluation, and clarity angles
- do not rewrite the paper for the authors; they identify weaknesses and demand repair
- may request new evidence, narrower claims, or clearer limitations

### Reproducibility Chair
- owns rerun readiness, traceability, and artifact dossier completeness
- can block release if evidence cannot be reconstructed from the package
- verifies that config, outputs, and decision logs align

## Decision Rights
- proposal framing: `academy-lead` approves, `distinguished-scholar` drafts
- workstream plans: `distinguished-scholar` assigns, seniors finalize
- execution details: seniors direct juniors
- critique findings: peer reviewers issue independently
- reproducibility disposition: `reproducibility-chair` issues pass/conditional/fail
- release disposition: `academy-lead` decides after scholar synthesis and review closure

## Required Handoff Contract
Every handoff must include the following sections in plain ASCII markdown:
- objective
- inputs received
- requested outputs
- constraints
- evidence expected
- deadline or return trigger
- open risks

If any section is missing, the recipient should request clarification before proceeding.

## Escalation Rules
- juniors escalate to the assigning senior after one blocked attempt or when evidence is missing
- seniors escalate to the distinguished scholar when a workstream change affects scope, claims, or evaluation design
- reviewers escalate to the academy lead only for unresolved governance conflicts or claim inflation
- reproducibility chair escalates directly to the academy lead when release blockers remain open

## Evidence Minimum for Advancement
A work item cannot advance to the next stage unless it includes:
- a named owner
- a dated artifact path
- a short method note
- explicit limitations
- at least one verification or review step already performed

## Review Closure Conditions
Reviewer findings remain open until one of the following is recorded:
- fixed with linked evidence
- accepted as limitation with revised claim language
- rejected by leadership with written rationale

No finding should disappear silently between rounds.

## Release Gating
A release candidate is ready only when all conditions are met:
- scholar synthesis package exists
- both peer reviews are logged
- reproducibility disposition is recorded
- unresolved high-severity findings are zero
- release dossier is complete enough for external inspection

## OpenClaw Packaging Implications
The package should preserve the following layout conventions:
- `/openclaw/agents/` for role-local prompts and operating files
- `/openclaw/config/` for mappings, schemas, and runtime-ready manifests
- `/openclaw/templates/` for reusable workflow and memo formats
- `/openclaw/dossiers/` for release-ready evidence bundles and examples
- top-level `V*_RELEASE_NOTES.md` and `V*_MASTER_INDEX.md` for navigation

## Failure Modes to Guard Against
- distinguished scholar acting as an unchecked bottleneck
- seniors delegating without measurable return criteria
- juniors producing outputs with no artifact trace
- reviewers giving abstract criticism without actionable closure tests
- reproducibility checks happening only at the end

## Recommended Cadence
- planning checkpoint before execution starts
- mid-round synthesis checkpoint before peer review
- post-review repair checkpoint
- final reproducibility and release checkpoint

## Audit Question Set
Before release, the team should be able to answer yes to each question:
- Can we identify who owns every major claim?
- Can we locate the artifacts behind each reported result?
- Can reviewers see what changed after critique?
- Can a third party reconstruct the release package flow?
- Can leadership justify both the scope and the limits of the claims?
