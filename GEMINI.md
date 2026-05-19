# Gemini CLI Usage

## Description
A CLI tool to track token usage and costs for Gemini CLI sessions with 100% data accuracy.

## Tech Stack
- Python 3 (Standard Library Only)

## Architecture: Smart Pricing Engine
- **Tiered Loading:** Local Cache -> LiteLLM community database -> Local Override (`pricing.json`) -> Hardcoded Defaults.
- **Fuzzy Matching:** Maps local model strings (e.g., `-preview`, `-canary`) to standardized pricing entries.
- **Auto-Update:** 24-hour cache TTL for remote pricing data.

## Conventions
- Follow [PEP 8](https://www.python.org/dev/peps/pep-0008/) for Python code.
- Ensure **zero external dependencies** are added. Use `urllib.request` and `json` for all networking/parsing.
- Output format must remain consistent with the simple bullet-point style.
- **No AI Attribution:** Do not include "Co-authored-by" or any other AI/agent attributions in commit messages.

## Release Process
- Update `pricing.json` if manual overrides are required.
- Update `README.md` if features change.
- Commit using Conventional Commits.
