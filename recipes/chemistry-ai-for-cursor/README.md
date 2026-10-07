# Chemistry AI for Cursor

> **Interactive setup:**  
> https://chemaiatlas.com/recipes/chemistry-ai-for-cursor/

Add a pinned, restricted RDKit MCP server to a Cursor project and verify molecular-analysis tools using reproducible SMILES prompts.

## You'll be able to

- Expose a restricted RDKit descriptor toolset to Cursor.
- Verify actual MCP tool calls in an Agent conversation.

## Scope

Cursor with Python 3.11 and the pinned TandemAI RDKit MCP server. Use stdio and a restricted five-tool descriptor allowlist.

## Stack

| Component | Type | Version / reference | Required |
| --- | --- | --- | --- |
| RDKit MCP Server (TandemAI) | mcp | 0.2.3 / commit 3a7000ae62e94e095ecd804a403fca12982570cb | Yes |
| RDKit | cheminformatics | 2025.3.1 | Yes |

## Compatibility

Cursor on macOS, Windows, or Linux; Python 3.10+.

## Privacy

RDKit calculations run locally; model handling depends on the Cursor account/model configuration and is not assumed to be offline.

## Setup

The maintained step-by-step installation and configuration guide is available on ChemAI Atlas:

https://chemaiatlas.com/recipes/chemistry-ai-for-cursor/

This repository keeps the public manifest and reviewable technical summary. Copyable configuration/code examples should only be added to `examples/` after they are checked against the current upstream versions.

## Acceptance test

Analyze aspirin using CalcMolFormula, MolWt, ExactMolWt, CalcTPSA, and CalcCrippenDescriptors and confirm real tool calls occurred.

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
