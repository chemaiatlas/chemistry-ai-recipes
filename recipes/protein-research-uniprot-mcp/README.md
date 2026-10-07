# Protein Research with UniProt MCP

> **Interactive setup:**  
> https://chemaiatlas.com/recipes/protein-research-uniprot-mcp/

Retrieve reviewed UniProtKB protein records through Claude Desktop, disambiguate organism and accession, and retain functional evidence and source identifiers.

## You'll be able to

- Search proteins by gene, organism, and review status.
- Retrieve annotated records with evidence and cross-references.

## Scope

Claude Desktop, Node.js 24+, and @cyanheads/uniprot-mcp-server 0.2.4. Public UniProt lookups require no API key.

## Stack

| Component | Type | Version / reference | Required |
| --- | --- | --- | --- |
| UniProt MCP (cyanheads) | mcp | 0.2.4 | Yes |

## Compatibility

Claude Desktop on macOS and Windows; Node.js 24+.

## Privacy

The MCP server is local, but it queries the external UniProt API and Claude receives returned annotations.

## Setup

The maintained step-by-step installation and configuration guide is available on ChemAI Atlas:

https://chemaiatlas.com/recipes/protein-research-uniprot-mcp/

This repository keeps the public manifest and reviewable technical summary. Copyable configuration/code examples should only be added to `examples/` after they are checked against the current upstream versions.

## Acceptance test

Retrieve a reviewed human UniProtKB record using taxon 9606 and retain the canonical accession, evidence labels, and cross-references.

A successful test should demonstrate the actual connected tool/runtime behavior. Do not substitute language-model memory for missing tool output.

## Verification

**Repository status:** Needs Review

This Recipe is published by ChemAI Atlas, but the GitHub representation is intentionally not marked `Verified` until it has been re-tested against a recorded environment.

Technical verification is not scientific validation.

## Upstream sources

- [UniProt MCP (cyanheads)](https://github.com/cyanheads/uniprot-mcp-server)

## Disclaimer

Third-party tools, models, APIs, data, installation methods, and pricing can change. Review upstream documentation, licenses, privacy terms, and scientific limitations before use. Independently validate outputs before using them for research conclusions or practical decisions.
