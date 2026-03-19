# Knowledge Base Spec (PDF + OCR + Citations)

## Goal
Maintain a trustworthy literature repository with:
- original PDFs preserved
- OCR outputs in Markdown and/or LaTeX
- provenance tracking (source, date, hash)
- citations in BibTeX

## Directory Layout
- `papers/incoming/` : new PDFs (unverified)
- `papers/processed/` : PDFs that completed OCR
- `papers/rejected/` : PDFs that failed processing
- `ocr_outputs/markdown/` : OCR markdown
- `ocr_outputs/latex/` : OCR LaTeX
- `citations/bibtex/` : `.bib`
- `citations/provenance/` : provenance logs

## Provenance Record (minimum)
- title (if known)
- source URL
- downloaded_at
- file_hash (sha256)
- license/terms note (if known)
- verification status

## OCR Quality Gate
- juniors run OCR + produce outputs
- seniors spot-check math/table fidelity
- mark as VERIFIED / PARTIAL / FAILED

## Usage
- literature and classic/high-citation works should be cached here
- paper writing must cite sources via the knowledge base when possible
