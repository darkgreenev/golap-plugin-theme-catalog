# Plugin Release Index Spec

## Goal

Define `plugins/<plugin-id>/index.json`.

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
- `packages`

## Package Fields

- `os`
- `arch`
- `url`
- `sha256`

## Example

```json
{
  "schema_version": 1,
  "id": "golap-seopro",
  "name": "goLaPress SEO Pro",
  "summary": "Advanced SEO plugin for goLaPress.",
  "latest_version": "0.1.0",
  "releases": [
    {
      "version": "0.1.0",
      "channel": "stable",
      "released_at": "2026-05-13T00:00:00Z",
      "min_core_version": "0.1.8",
      "max_core_version": "",
      "changelog_url": "https://example.com/plugins/golap-seopro/versions/0.1.0/changelog.md",
      "packages": [
        {
          "os": "linux",
          "arch": "amd64",
          "url": "https://example.com/plugins/golap-seopro/versions/0.1.0/golap-seopro-linux-amd64.zip",
          "sha256": "..."
        }
      ]
    }
  ]
}
```

## Done When

- core can decide whether and how to install a plugin release on the current machine
