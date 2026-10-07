# Build a Local Chemistry Assistant with Ollama + RDKit

> **Interactive setup:**  
> https://chemaiatlas.com/recipes/local-chemistry-assistant-ollama-rdkit/

Calculate molecular properties with RDKit and explain the recorded results using a local Ollama model, through an explicit Python bridge.

## You'll be able to

- Compute formula, molecular weight, and TPSA locally.
- Explain recorded calculations using a local language model.

## Scope

Python 3.11 and RDKit 2025.3.1 with a local Ollama runtime. A simple Python bridge computes deterministic descriptors and asks a local model to explain recorded results.

## Stack

| Component | Type | Version / reference | Required |
| --- | --- | --- | --- |
| RDKit | cheminformatics | 2025.3.1 | Yes |
| Ollama | local-ai-runtime | current | Yes |
| qwen2.5:3b | language-model | Ollama model | Yes |

## Compatibility

Python 3.11+ and Ollama on macOS, Windows, or Linux.

## Privacy

After installers and model files are downloaded, the reference workflow uses loopback-only local inference and local RDKit calculations.

## Setup

The maintained step-by-step installation and configuration guide is available on ChemAI Atlas:

https://chemaiatlas.com/recipes/local-chemistry-assistant-ollama-rdkit/

This repository keeps the public manifest and reviewable technical summary. Copyable configuration/code examples should only be added to `examples/` after they are checked against the current upstream versions.

## Acceptance test

Calculate descriptors for a public molecule and confirm the model explanation is based on the printed RDKit JSON rather than invented values.

A successful test should demonstrate the actual connected tool/runtime behavior. Do not substitute language-model memory for missing tool output.

## Verification

**Repository status:** Needs Review

This Recipe is published by ChemAI Atlas, but the GitHub representation is intentionally not marked `Verified` until it has been re-tested against a recorded environment.

Technical verification is not scientific validation.

## Upstream sources

- [RDKit](https://www.rdkit.org/)
- [Ollama](https://ollama.com/)
- [qwen2.5:3b](https://ollama.com/library/qwen2.5)

## Disclaimer

Third-party tools, models, APIs, data, installation methods, and pricing can change. Review upstream documentation, licenses, privacy terms, and scientific limitations before use. Independently validate outputs before using them for research conclusions or practical decisions.
