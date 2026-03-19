# Literature Intake Workflow (Search → Download → Preserve PDF → OCR → QA → Index)

## Goal
Turn "find classic/high-citation/new papers" into a governed pipeline where PDFs and OCR outputs become first-class research artifacts.

## Step 0: Search Strategy
- define topic scope
- define inclusion criteria (classic/high-citation/new)
- record search queries and timestamps

## Step 1: Acquire PDFs
- prefer official sources (publisher, arXiv, author page)
- store PDFs into `knowledge_base/papers/incoming/`

## Step 2: Provenance Record
For each PDF create a provenance record JSON:
- source_url
- downloaded_at
- sha256
- status = UNVERIFIED

## Step 3: OCR
- generate markdown and latex outputs
- save to `ocr_outputs/markdown/` and `ocr_outputs/latex/`

## Step 4: QA
- juniors run QA checklist
- seniors spot-check key sections (math/tables)
- update status to VERIFIED/PARTIAL/FAILED

## Step 5: Citation
- add/update BibTeX entry in `citations/bibtex/`

## Step 6: Index
- update a simple index file mapping paper_id → pdf path → ocr paths → provenance

## Exit Gate
No paper is used as a strong evidence source unless provenance is at least PARTIAL and key sections have been spot-checked.
