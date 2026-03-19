# OCR Processing Workflow

## Purpose
Convert incoming PDFs to machine-readable formats for citation and analysis.

## Pipeline
```
[papers/incoming/*.pdf]
    → [OCR Engine]
    → [Post-processing]
    → [ocr_outputs/markdown/ + ocr_outputs/latex/]
    → [Provenance Update]
```

## Step 1: Detection
- Monitor `papers/incoming/` for new PDFs
- Trigger on file creation

## Step 2: OCR Execution
- **Standard PDFs**: pdfplumber/pymupdf
- **Scanned papers**: OCRmyPDF/marker
- **Equations**: Special LaTeX handling

## Step 3: Output Generation
- `*.md`: Markdown format
- `*.tex`: LaTeX with math
- `*.json`: Metadata (title, authors, year)

## Step 4: Verification
- Senior reviews sample accuracy
- Mark as `verified` or reprocess

## Error Handling
- Failed PDFs → `papers/rejected/`
- Log reason and notify for manual handling
