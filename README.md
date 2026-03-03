# LogLiefje Keywords

Shared keyword database for [LogLiefje AI](https://github.com/MachoDrone/LogLiefje) error analysis.

## Files

| File | Purpose |
|------|---------|
| `keywords.json` | Error keywords with severity, category, and metadata |
| `patterns.json` | Multi-line regex patterns for stack traces and event sequences |
| `false-positives.json` | Patterns to exclude from error detection |

## How it works

LogLiefje AI containers pull this repo on each run, apply known keywords for fast deterministic scanning, then use an LLM to discover new patterns. New keywords are pushed back automatically.

## Format

Keywords include confidence scores (0-1), occurrence counts, and provenance (manual seed vs AI-discovered).

## Contributing

This repo is primarily AI-maintained. Human review is welcome for quality control.
