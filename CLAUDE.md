# CLAUDE.md — awesome-video-generation

## What this list is

A curated directory of AI video-generation tools that developers can integrate today: text-to-video APIs, avatar/talking-head platforms, open-weight models, real-time video, and the surrounding infrastructure.

## Scope

**Include**
- Commercial text-to-video and image-to-video APIs with developer access.
- Real-time and interactive video platforms.
- Avatar/talking-head and motion-transfer APIs.
- Video enhancement (upscaling, restoration) and video understanding APIs.
- Open-weight video models with hosted inference, Docker, or `diffusers` support.
- SDKs and client libraries for integrating video generation into apps.
- GPU platforms, video processing tooling, storage/CDN services, and playback libraries.
- Evaluation benchmarks and leaderboards.
- Template/demo projects and reference implementations.

**Exclude**
- Research papers without runnable code or an API.
- Paywalled tools that gate developer access.
- Duplicate entries.
- Self-promotional content with no developer value.

**Inclusion requirements (every entry)**
- Public product or docs page; URL resolves.
- Activity signal within the last 12 months (commit, release, docs update).
- Either a public API or an open-source install path.

## Files in this repo

- `entries.yaml` — source of truth. Only hand-edit this file.
- `categories.yaml` — the section taxonomy. Authoritative for what slugs are valid.
- `header.md`, `footer.md` — hand-written prose bracketing the generated list.
- `README.md`, `llms.txt` — **generated**. Do not edit.
- `CONTRIBUTING.md` — instructions for human PR authors.
- `.enrichment-cache.json` — local star-count cache; gitignored.

## Schema

Full schema at `~/awesome-lists/_shared/schema.json`. Required: `name`, `url`, `description`, `category`, `last_verified`. Optional: `docs_url`, `github`, `sdks`, `license`, `tags`, `b2_integration`.

`b2_integration` is a URL pointing to docs for the tool's B2 integration. Leave as the empty string `""` when none exists yet. When a new integration ships, set this field and drop the tool from `~/awesome-lists/_internal/priorities.yaml`.

`category` must be a slug defined in `categories.yaml` — validate.py will reject anything else. The `infrastructure-and-deployment` category uses `tags` (`gpu`, `video-processing`, `storage-delivery`, `playback`) to preserve the sub-grouping from the original hand-edited README.

## Workflow

Adding or updating an entry:

1. Edit `entries.yaml` only.
2. `python ~/awesome-lists/scripts/validate.py --repo .`
3. (Optional) `python ~/awesome-lists/scripts/enrich.py --repo .`
4. `python ~/awesome-lists/scripts/generate.py --repo .`
5. Commit `entries.yaml`, `README.md`, `llms.txt` together. One entry per PR.

## Hard rules

- Never edit `README.md` or `llms.txt` by hand — any manual edit is overwritten on the next `generate.py` run.
- Never commit `.enrichment-cache.json`.
- Never delete an entry outright. If a tool is dead or discontinued, tag it `tags: [needs-review]` and file a note in `~/awesome-lists/_tasks/`.

## Good vs. rejected entries

**Good**
```yaml
- name: Runway (Gen-4)
  url: https://runwayml.com/api
  docs_url: https://docs.dev.runwayml.com
  description: Text-to-video and image-to-video with Gen-4 Turbo. Async task-based REST API with polling helpers.
  category: text-to-video-apis
  sdks:
    - {language: Python, url: https://pypi.org/project/runwayml/}
    - {language: Node, url: https://github.com/runwayml/sdk-node}
  b2_integration: ""
  last_verified: 2026-03-01
```

**Rejected**
- Out of scope: an LLM-only tool with no video capability.
- Vaporware: a landing page with a waitlist, no docs, no repo.
- Dead link: homepage 404s or repo archived >12 months ago with no successor.
