# `catalog.json` Spec

## Goal

Define the top-level catalog file consumed by goLaPress core.

## Required Fields

- `schema_version`
- `generated_at`
- `plugins`
- `themes`

## Plugin Entry Fields

- `id`
- `name`
- `summary`
- `latest_version`
- `index_url`

## Theme Entry Fields

- `id`
- `name`
- `summary`
- `latest_version`
- `index_url`

## Example

```json
{
  "schema_version": 1,
  "generated_at": "2026-05-13T00:00:00Z",
  "plugins": [
    {
      "id": "golap-seopro",
      "name": "goLaPress SEO Pro",
      "summary": "Advanced SEO plugin for goLaPress.",
      "latest_version": "0.1.0",
      "index_url": "https://example.com/plugins/golap-seopro/index.json"
    }
  ],
  "themes": []
}
```

## Done When

- core can discover every installable plugin and theme from one file
