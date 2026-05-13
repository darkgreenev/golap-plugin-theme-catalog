# Catalog Repo Layout

## Goal

Define the expected folder structure for the public release catalog repository.

## Required Layout

```text
catalog.json
plugins/
  <plugin-id>/
    index.json
    versions/
      <version>/
        <artifact files>
        checksums.txt
        changelog.md
themes/
  <theme-id>/
    index.json
    versions/
      <version>/
        <artifact files>
        checksums.txt
        changelog.md
docs/
```

## Rules

- one directory per plugin id
- one directory per theme id
- one release directory per version
- no source code check-ins
- only release artifacts and metadata

## Done When

- catalog repo layout is stable and easy to validate automatically
