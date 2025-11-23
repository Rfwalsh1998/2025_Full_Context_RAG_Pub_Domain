# 2025 Full-Context RAG (Public Domain)

A public-domain knowledge object for 2025 designed for Retrieval-Augmented Generation (RAG) systems. The dataset separates structured timelines, thematic narratives, and full-text source documents so language models can ground answers reliably.

## Structure

- `data/2025/meta.json` – high-level metadata, version, and license.
- `data/2025/narrative/themes.json` – cross-cutting themes for the year.
- `data/2025/timeline/` – month-level JSON files with summaries and events, plus a `schema` reference in `index.json`.
- `data/2025/source_documents/` – full-text reference documents with minimal front matter.
- `LICENSE` – CC0 1.0 Universal dedication.

## Notes for LLM Ingestion

- Dates are ISO-8601; categories are single-word domains (e.g., `Politics`, `Technology`).
- All content is in English and released under CC0. Cite the `Document-Title` when quoting source documents.
- Timeline files are intentionally concise; source documents capture richer narrative context for retrieval.

_Last updated: 2025-11-23._
