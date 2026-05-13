# Release Publish Workflow

## Goal

Define how private source repos publish public release artifacts into this catalog.

## Workflow

1. build release artifacts in private source repo CI
2. package plugin or theme contents
3. generate checksums
4. create or update changelog file
5. copy artifacts into the correct `versions/<version>/` directory
6. update the package index JSON
7. update `catalog.json`
8. validate the catalog repo
9. push or merge catalog changes

## Rules

- never publish source code here unless explicitly intended
- keep package metadata aligned with manifest versions
- validate all URLs and checksums before push

## Done When

- every release follows one repeatable publish path
