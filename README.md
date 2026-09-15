# norsk-literature

Curated Norwegian reading stories released as importable Markdown artifacts.

This repository contains results only. The collection pipeline, source cache,
translation responses, prompts and review evidence remain private.

Each file under `stories/` is one story. The Norsk app creates its own reading
pages after URL ingestion, so books do not need `part-1`, `part-2` or chapter
files.

Story-specific source and license information is kept in each file's frontmatter
and in [`ATTRIBUTION.md`](ATTRIBUTION.md). See [`catalog.json`](catalog.json)
for the machine-readable index.

The `import-manifest.json` handover lists the pinned raw story URLs for the app importer. After a release commit is tagged, run:

```bash
uv run python -m flyt.commands.reading_ingest \
  --manifest https://raw.githubusercontent.com/Chalvin96/norsk-literature/<ref>/import-manifest.json
```
