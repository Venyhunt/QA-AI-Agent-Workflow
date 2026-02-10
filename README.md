# SRD → QA Test Case Automation (n8n)

## Goal
Automatically analyze Software Requirement Documents (SRDs)
and generate redundant-aware QA test cases.

## Tech Stack
- n8n (self-hosted, Docker)
- OpenAI API
- PDF SRDs

## Progress

### Phase 1 — Read SRD (DONE)
- n8n workflow reads SRD PDF from disk
- Docker + volume permissions configured
- Output: binary PDF metadata

### Phase 2 — Extract Raw Text (NEXT)
- Convert PDF binary → raw text

## Notes
This project is built incrementally.
Done > perfect.
