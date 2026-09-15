# norsk-literature

Curated Norwegian reading stories released from the private norskreading pipeline. The repository contains release artifacts only; it does not contain the pipeline, source cache, prompts or review evidence.

Release: `2026.09.16-all`

Each Markdown file is one importable story. The app creates its own reading pages after URL ingestion, so books do not need part files. Source readings may intentionally have no CEFR level and are marked level_status: ungraded.

To import a story, use its HTTPS raw GitHub URL with the app's `reading_ingest` command. Pin that URL to a release commit or tag.
