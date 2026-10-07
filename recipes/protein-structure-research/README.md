# Protein Structure Research Stack

> **Interactive setup:**  
> https://chemaiatlas.com/recipes/protein-structure-research/

Combine RCSB structure records with UniProt protein annotations, inspect method/resolution and entity mappings, and download a traceable mmCIF file.

## You'll be able to

- Retrieve PDB method, resolution, and polymer records.
- Cross-check UniProt accessions and download traceable mmCIF files.

## Scope

Claude Desktop; Node.js 24+ for UniProt MCP; a separate Python 3.13+ environment for the pinned RCSB MCP. Preserve structure metadata, entity mappings, and downloaded mmCIF provenance.

## Stack

| Component | Type | Version / reference | Required |
| --- | --- | --- | --- |
| UniProt MCP (cyanheads) | mcp | 0.2.4 | Yes |
| RCSB MCP (cnyambura) | mcp | 0.1.0 / commit df04c993c31f43d69d6273737bda2de39ace0850 | Yes |
| RCSB PDB Data API | api | live API | Yes |

## Compatibility

Claude Desktop plus Node.js 24+ and a separate Python 3.13+ RCSB MCP environment.

## Privacy

Both APIs and Claude require external network services.

## Setup

The maintained step-by-step installation and configuration guide is available on ChemAI Atlas:

https://chemaiatlas.com/recipes/protein-structure-research/

This repository keeps the public manifest and reviewable technical summary. Copyable configuration/code examples should only be added to `examples/` after they are checked against the current upstream versions.

## Acceptance test

Inspect a known PDB entry, record method/resolution and polymer entity mappings, cross-check UniProt, and download the mmCIF to a new directory.

A successful test should demonstrate the actual connected tool/runtime behavior. Do not substitute language-model memory for missing tool output.

## Verification

**Repository status:** Needs Review

This Recipe is published by ChemAI Atlas, but the GitHub representation is intentionally not marked `Verified` until it has been re-tested against a recorded environment.

Technical verification is not scientific validation.

## Upstream sources

- [UniProt MCP (cyanheads)](https://github.com/cyanheads/uniprot-mcp-server)
- [RCSB MCP (cnyambura)](https://github.com/cnyambura/rcsb-mcp)
- [RCSB PDB Data API](https://data.rcsb.org/)

## Disclaimer

Third-party tools, models, APIs, data, installation methods, and pricing can change. Review upstream documentation, licenses, privacy terms, and scientific limitations before use. Independently validate outputs before using them for research conclusions or practical decisions.
