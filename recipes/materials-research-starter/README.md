# Materials Research Starter Stack

> **Interactive setup:**  
> https://chemaiatlas.com/recipes/materials-research-starter/

Use the current Materials Project Python API to fetch a small material summary, preserve identifiers and units, and separate computed properties from experimental evidence.

## You'll be able to

- Query a specified Materials Project material using limited fields.
- Preserve provenance, units, IDs, and missing values.

## Scope

Python 3.11 and mp-api 0.46.5. Requires a Materials Project account/API key. Use mp_api.client.MPRester rather than the legacy client.

## Stack

| Component | Type | Version / reference | Required |
| --- | --- | --- | --- |
| Materials Project API | api | mp-api 0.46.5 / current API | Yes |

## Compatibility

Python 3.11+ on macOS, Windows, and Linux.

## Privacy

Data retrieval uses an external authenticated service and is not a fully offline workflow.

## Setup

The maintained step-by-step installation and configuration guide is available on ChemAI Atlas:

https://chemaiatlas.com/recipes/materials-research-starter/

This repository keeps the public manifest and reviewable technical summary. Copyable configuration/code examples should only be added to `examples/` after they are checked against the current upstream versions.

## Acceptance test

Retrieve silicon mp-149 with a limited field set and preserve material ID, retrieval date, units, and missing values.

A successful test should demonstrate the actual connected tool/runtime behavior. Do not substitute language-model memory for missing tool output.

## Verification

**Repository status:** Needs Review

This Recipe is published by ChemAI Atlas, but the GitHub representation is intentionally not marked `Verified` until it has been re-tested against a recorded environment.

Technical verification is not scientific validation.

## Upstream sources

- [Materials Project API](https://materialsproject.org/api)

## Disclaimer

Third-party tools, models, APIs, data, installation methods, and pricing can change. Review upstream documentation, licenses, privacy terms, and scientific limitations before use. Independently validate outputs before using them for research conclusions or practical decisions.
