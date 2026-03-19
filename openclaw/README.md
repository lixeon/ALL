# OpenClaw Academic Lobster Lab

This package implements a hierarchical academic research team configuration for OpenClaw, and makes two workflows first-class:

1) **Paper writing with reviewer-driven iteration** (draft → peer review → REJECT/MAJOR/MINOR/ACCEPT → revision → resubmit), with concrete demo artifacts.
2) **Literature knowledge base governance** (preserve PDFs + OCR to MD/LaTeX + provenance + BibTeX), with an explicit intake workflow.

## Team Structure (9-agent core)
- academy lead
- distinguished scholar
- senior researcher 1
- senior researcher 2
- junior researcher 1
- junior researcher 2
- peer reviewer 1
- peer reviewer 2
- reproducibility chair

## Publishing Extensions
- paper-writer
- latex-editor

## Design Principles
- scholarly hierarchy with explicit delegation
- strong separation between creation, execution, critique, and reproducibility governance
- iteration with inspectable artifacts (decisions, checklists, response letters, change logs)
- reproducibility is gated, not promised

## Where to Start
- `dossiers/examples/demo_paper_cycle/README.md` (end-to-end reject→revision demo)
- `templates/paper_iteration/paper_iteration_workflow.md` (workflow spec)
- `knowledge_base/KNOWLEDGE_BASE_SPEC.md` + `knowledge_base/workflows/literature_intake_workflow.md` (KB governance)

## Notes
This is a project-side configuration and workflow package. Live OpenClaw gateway schema alignment remains environment-dependent.
