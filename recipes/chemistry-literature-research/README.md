# Chemistry Literature Research Stack

> **Interactive setup:**  
> https://chemaiatlas.com/recipes/chemistry-literature-research/

Build a traceable literature workflow for medicinal and biological chemistry: search PubMed, fetch article records, and summarize only the retrieved evidence with identifiers.

## You'll be able to

- Search biomedical chemistry literature with explicit queries and dates.
- Retrieve article evidence while retaining PMID/DOI provenance.

## Scope

Claude Desktop, Node.js 24+, and @cyanheads/pubmed-mcp-server 2.10.20. Focus on traceable PubMed metadata/abstract retrieval with PMID/DOI provenance.

## Stack

| Component | Type | Version / reference | Required |
| --- | --- | --- | --- |
| PubMed MCP (cyanheads) | mcp | 2.10.20 | Yes |

## Compatibility

Claude Desktop on macOS and Windows; Node.js 24+.

## Privacy

The MCP process is local but it accesses external literature databases, and model processing is cloud-based.

## Setup

The maintained step-by-step installation and configuration guide is available on ChemAI Atlas:

https://chemaiatlas.com/recipes/chemistry-literature-research/

This repository keeps the public manifest and reviewable technical summary. Copyable configuration/code examples should only be added to `examples/` after they are checked against the current upstream versions.

## Acceptance test

Run a narrow literature query, fetch a small set of records, and verify that the answer cites only retrieved evidence and preserves identifiers.

A successful test should demonstrate the actual connected tool/runtime behavior. Do not substitute language-model memory for missing tool output.

## Verification

**Repository status:** Needs Review

This Recipe is published by ChemAI Atlas, but the GitHub representation is intentionally not marked `Verified` until it has been re-tested against a recorded environment.

Technical verification is not scientific validation.

## Upstream sources

- [PubMed MCP (cyanheads)](https://github.com/cyanheads/pubmed-mcp-server)

## Disclaimer

Third-party tools, models, APIs, data, installation methods, and pricing can change. Review upstream documentation, licenses, privacy terms, and scientific limitations before use. Independently validate outputs before using them for research conclusions or practical decisions.
