# Catalog Validation Tooling

## Goal

Define the scripts or checks needed to validate this catalog repository before publishing changes.

## Validation Requirements

- `catalog.json` parses
- each listed plugin index exists
- each listed theme index exists
- each artifact file referenced by JSON exists
- each checksum matches the artifact
- no duplicate ids
- no duplicate versions inside a package index

## Suggested Tooling

- one validation script runnable locally and in CI
- fail fast with clear file path and reason

## Done When

- broken catalog metadata cannot be merged quietly
