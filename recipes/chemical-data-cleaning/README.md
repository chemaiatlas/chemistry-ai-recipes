# Chemical Data Cleaning Stack

> **Interactive setup:**  
> https://chemaiatlas.com/recipes/chemical-data-cleaning/

Validate and canonicalize SMILES with RDKit without dropping original rows; flag duplicates and optionally enrich valid entries with PubChem identifiers.

## You'll be able to

- Preserve original data while validating SMILES.
- Flag canonical duplicates.
- Optionally retain PubChem CIDs without dropping unmatched rows.

## Scope

Python 3.11 with RDKit 2025.3.1; PubChemPy 1.0.5 is optional. Preserve original rows, label invalid/missing SMILES, and avoid silent salt, charge, or tautomer normalization.

## Stack

| Component | Type | Version / reference | Required |
| --- | --- | --- | --- |
| RDKit | cheminformatics | 2025.3.1 | Yes |
| PubChemPy | api-client | 1.0.5 | Optional |

## Compatibility

Python 3.11+ on macOS, Windows, and Linux.

## Privacy

Baseline cleaning is local. Enabling PubChem enrichment sends valid canonical SMILES to an external service.

## Setup

The maintained step-by-step installation and configuration guide is available on ChemAI Atlas:

https://chemaiatlas.com/recipes/chemical-data-cleaning/

This repository keeps the public manifest and reviewable technical summary. Copyable configuration/code examples should only be added to `examples/` after they are checked against the current upstream versions.

## Acceptance test

Use a small CSV containing equivalent SMILES, one invalid entry, one empty entry, and a salt. Confirm row count is preserved and duplicates are flagged.

A successful test should demonstrate the actual connected tool/runtime behavior. Do not substitute language-model memory for missing tool output.

## Verification

**Repository status:** Needs Review

This Recipe is published by ChemAI Atlas, but the GitHub representation is intentionally not marked `Verified` until it has been re-tested against a recorded environment.

Technical verification is not scientific validation.

## Upstream sources

- [RDKit](https://www.rdkit.org/)
- [PubChemPy](https://docs.pubchempy.org/)

## Disclaimer

Third-party tools, models, APIs, data, installation methods, and pricing can change. Review upstream documentation, licenses, privacy terms, and scientific limitations before use. Independently validate outputs before using them for research conclusions or practical decisions.
