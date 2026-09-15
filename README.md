# norsk-literature

Curated Norwegian reading stories released as importable Markdown artifacts.

This repository contains results only. The collection pipeline, source cache,
translation responses, prompts and review evidence remain private.

Each file under stories/ is one story. The Norsk app creates its own reading
pages after URL ingestion, so books do not need part-1, part-2 or chapter
files.

Story-specific source and license information is kept in each file's frontmatter
and in [ATTRIBUTION.md](ATTRIBUTION.md). See [catalog.json](catalog.json)
for the machine-readable index.

Import a story by passing its raw GitHub URL directly to the deployed importer:

`ash
uv run python -m flyt.commands.reading_ingest \
  https://raw.githubusercontent.com/Chalvin96/norsk-literature/main/stories/<group>/<slug>.md
`

The path values in catalog.json are the complete list of current story
files. The importer accepts one or more story URLs as positional arguments.
