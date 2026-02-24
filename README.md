# RAL-Version

External version configuration for RotatingartLauncher update checks.

## File

- `version.json`: primary update manifest consumed by launcher.

## Schema (v1)

```json
{
  "schemaVersion": 1,
  "channel": "stable",
  "latest": {
    "version": "1.9.1",
    "releaseName": "RotatingartLauncher v1.9.1",
    "publishedAt": "2026-02-24T12:00:00Z",
    "description": "...",
    "changelog": ["..."],
    "downloads": {
      "github": "https://...apk",
      "cloud": "https://..."
    },
    "releasePage": "https://..."
  }
}
```

## Notes

- `downloads.github` should preferably be a direct APK URL.
- `downloads.cloud` can be a cloud-drive share page.
- Keep `version` strictly increasing to trigger update prompts.
