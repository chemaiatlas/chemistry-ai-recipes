# Retrosynthesis Starter Stack

> **Interactive setup:**  
> https://chemaiatlas.com/recipes/retrosynthesis-starter/

Install an isolated AiZynthFinder environment, download its public policy/template/stock files, and run a bounded, traceable retrosynthesis search.

## You'll be able to

- Prepare public policy/template/stock data with provenance.
- Run a bounded local search and inspect route statistics.

## Scope

AiZynthFinder 4.4.1 in its own Python 3.11 environment. Keep it separate from other Recipe environments because dependency ranges differ.

## Stack

| Component | Type | Version / reference | Required |
| --- | --- | --- | --- |
| AiZynthFinder | retrosynthesis | 4.4.1 | Yes |

## Compatibility

Python 3.10-3.12 on macOS, Windows, and Linux; Recipe uses Python 3.11.

## Privacy

Policy/template/stock downloads require internet access, but the reference search runs locally with downloaded data.

## Setup

The maintained step-by-step installation and configuration guide is available on ChemAI Atlas:

https://chemaiatlas.com/recipes/retrosynthesis-starter/

This repository keeps the public manifest and reviewable technical summary. Copyable configuration/code examples should only be added to `examples/` after they are checked against the current upstream versions.

## Acceptance test

Run a bounded search using the configured public policy and stock. Treat zero routes as a valid result rather than inventing chemistry.

A successful test should demonstrate the actual connected tool/runtime behavior. Do not substitute language-model memory for missing tool output.

## Verification

**Repository status:** Needs Review

This Recipe is published by ChemAI Atlas, but the GitHub representation is intentionally not marked `Verified` until it has been re-tested against a recorded environment.

Technical verification is not scientific validation.

## Upstream sources

- [AiZynthFinder](https://github.com/MolecularAI/aizynthfinder)

## Disclaimer

Third-party tools, models, APIs, data, installation methods, and pricing can change. Review upstream documentation, licenses, privacy terms, and scientific limitations before use. Independently validate outputs before using them for research conclusions or practical decisions.
