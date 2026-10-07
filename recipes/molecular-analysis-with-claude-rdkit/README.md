# Molecular Analysis with Claude + RDKit MCP

> **Interactive setup:**  
> https://chemaiatlas.com/recipes/molecular-analysis-with-claude-rdkit/

Connect Claude Desktop to a local RDKit MCP server to calculate molecular formula, molecular weights, TPSA and Crippen descriptors from SMILES, with reproducible setup and acceptance checks.

## You'll be able to

- Calculate formula and average/exact molecular weight from SMILES.
- Calculate TPSA and Crippen logP/molar refractivity.
- Inspect actual tool calls against an acceptance baseline.

## Scope

Claude Desktop selects tools; the pinned TandemAI RDKit MCP server performs local calculations. Use Python 3.11, stdio transport, and only the five descriptor tools required by the Recipe.

## Stack

| Component | Type | Version / reference | Required |
| --- | --- | --- | --- |
| RDKit MCP Server (TandemAI) | mcp | 0.2.3 / commit 3a7000ae62e94e095ecd804a403fca12982570cb | Yes |
| RDKit | cheminformatics | 2025.3.1 | Yes |

## Compatibility

Claude Desktop on macOS and Windows; Python 3.10+ (Recipe uses 3.11).

## Privacy

RDKit runs locally, but prompts and tool results are processed by Claude's cloud service. This is not a fully offline workflow.

## Setup

The maintained step-by-step installation and configuration guide is available on ChemAI Atlas:

https://chemaiatlas.com/recipes/molecular-analysis-with-claude-rdkit/

This repository keeps the public manifest and reviewable technical summary. Copyable configuration/code examples should only be added to `examples/` after they are checked against the current upstream versions.

## Acceptance test

Analyze aspirin with the five allowed RDKit tools and compare deterministic values against the acceptance baseline shown on ChemAI Atlas.

A successful test should demonstrate the actual connected tool/runtime behavior. Do not substitute language-model memory for missing tool output.

## Verification

**Repository status:** Needs Review

This Recipe is published by ChemAI Atlas, but the GitHub representation is intentionally not marked `Verified` until it has been re-tested against a recorded environment.

Technical verification is not scientific validation.

## Upstream sources

- [RDKit MCP Server (TandemAI)](https://github.com/tandemai-inc/rdkit-mcp-server)
- [RDKit](https://www.rdkit.org/)

## Disclaimer

Third-party tools, models, APIs, data, installation methods, and pricing can change. Review upstream documentation, licenses, privacy terms, and scientific limitations before use. Independently validate outputs before using them for research conclusions or practical decisions.
