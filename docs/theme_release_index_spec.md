# Theme Release Index Spec

## Goal

Define `themes/<theme-id>/index.json`.

## Required Root Fields

- `schema_version`
- `id`
- `name`
- `summary`
- `latest_version`
- `releases`

## Release Fields

- `version`
- `channel`
- `released_at`
- `min_core_version`
- `max_core_version`
- `changelog_url`
- `package`
- `sha256`
- `screenshot_url` optional

## Done When

- core can install and update themes from one predictable contract
