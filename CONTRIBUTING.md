# Contributing

Thanks for your interest in contributing. This list is the single source for developer-focused AI video-generation tools; small, careful PRs keep it useful.

## How to contribute

1. Fork this repo.
2. Edit **`entries.yaml`** only. Do not edit `README.md` or `llms.txt` — those are regenerated from `entries.yaml`.
3. Place your entry in the appropriate category (see `categories.yaml` for the list of valid category slugs).
4. Open a PR. One entry per PR.

A maintainer will validate your entry, regenerate `README.md` + `llms.txt`, and merge.

## What belongs in the list

**We accept**
- Commercial text-to-video and image-to-video APIs with developer access.
- Real-time and interactive video platforms.
- Avatar/talking-head and motion-transfer APIs.
- Video enhancement and video understanding APIs.
- Open-weight models with hosted inference, Docker, or `diffusers` support.
- SDKs, client libraries, GPU platforms, storage/CDN services, playback libraries.
- Evaluation benchmarks and leaderboards.
- Template/demo projects and reference implementations.

**We don't accept**
- Research papers without runnable code or an API.
- Paywalled tools without developer access.
- Duplicate entries.
- Self-promotional content with no developer value.

## Inclusion requirements

- Public product or documentation page; URL resolves.
- Activity signal within the last 12 months.
- Either a public API or an open-source install path.

## Entry format

Every entry is a YAML object in `entries.yaml`. Example:

```yaml
- name: Runway (Gen-4)
  url: https://runwayml.com/api
  docs_url: https://docs.dev.runwayml.com
  description: Text-to-video and image-to-video with Gen-4 Turbo.
  category: text-to-video-apis
  sdks:
    - {language: Python, url: https://pypi.org/project/runwayml/}
    - {language: Node, url: https://github.com/runwayml/sdk-node}
  b2_integration: ""
  last_verified: 2026-04-17
```

### Fields

| Field | Required | Notes |
|---|---|---|
| `name` | yes | Display name. |
| `url` | yes | Primary homepage or repo URL. |
| `description` | yes | One sentence, ≤300 chars. |
| `category` | yes | Slug from `categories.yaml`. |
| `last_verified` | yes | ISO date the entry was last checked. |
| `docs_url` |  | Developer documentation, if different from `url`. |
| `github` |  | `owner/repo` slug, used for star enrichment. |
| `sdks` |  | Array of `{language, url}`. |
| `license` |  | SPDX short id. |
| `tags` |  | Kebab-case tags. For `infrastructure-and-deployment`, common tags are `gpu`, `video-processing`, `storage-delivery`, `playback`. |
| `b2_integration` |  | URL to docs for the tool's Backblaze B2 integration. Blank if none. |

## What happens after you submit

A maintainer validates the entry against the schema, runs star enrichment, regenerates the README, and merges. If your entry is out of scope or missing information, you'll get feedback on the PR.

## Code of conduct

This project follows standard open-source community norms. Be kind, be constructive, focus on the contribution.
