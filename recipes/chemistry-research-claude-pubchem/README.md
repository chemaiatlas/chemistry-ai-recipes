# Chemistry Research with Claude + PubChem

> **Interactive setup:**  
> https://chemaiatlas.com/recipes/chemistry-research-claude-pubchem/

Resolve chemical names to PubChem identifiers and retrieve traceable compound properties from Claude Desktop through a locally installed PubChem MCP server.

## You'll be able to

- Resolve names and identifiers to PubChem CIDs.
- Retrieve compound details while preserving sources and missing values.

## Scope

Claude Desktop with Node.js 24+ and @cyanheads/pubchem-mcp-server 0.6.5. Resolve names/identifiers to CIDs and retrieve traceable PubChem properties.

## Stack

| Component | Type | Version / reference | Required |
| --- | --- | --- | --- |
| PubChem MCP (cyanheads) | mcp | 0.6.5 / commit 1b179c5043345b9029b269980ac4ad5c0dbad15b | Yes |
| PubChem PUG REST | api | live API | Yes |

## Compatibility

Claude Desktop on macOS and Windows; Node.js 24+.

## Privacy

The MCP server runs locally but queries public PubChem APIs, while the conversation is processed by Claude.

## Setup

The maintained step-by-step installation and configuration guide is available on ChemAI Atlas:

https://chemaiatlas.com/recipes/chemistry-research-claude-pubchem/

This repository keeps the public manifest and reviewable technical summary. Copyable configuration/code examples should only be added to `examples/` after they are checked against the current upstream versions.

## Acceptance test

Resolve a common public compound such as aspirin, retrieve its CID and selected properties, and record retrieval date and source.

A successful test should demonstrate the actual connected tool/runtime behavior. Do not substitute language-model memory for missing tool output.

## Verification

**Repository status:** Needs Review

This Recipe is published by ChemAI Atlas, but the GitHub representation is intentionally not marked `Verified` until it has been re-tested against a recorded environment.

Technical verification is not scientific validation.

## Upstream sources

- [PubChem MCP (cyanheads)](https://github.com/cyanheads/pubchem-mcp-server)
- [PubChem PUG REST](https://pubchem.ncbi.nlm.nih.gov/docs/pug-rest)

## Disclaimer

Third-party tools, models, APIs, data, installation methods, and pricing can change. Review upstream documentation, licenses, privacy terms, and scientific limitations before use. Independently validate outputs before using them for research conclusions or practical decisions.
