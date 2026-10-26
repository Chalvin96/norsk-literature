# norsk-literature

Curated reading stories released from the private norskreading pipeline. The repository contains release artifacts only; it does not contain the pipeline, source cache, prompts or review evidence.

Release: `release-2026.09.16-openverse-facts`

Each Markdown file is one importable story. The app creates its own reading pages after URL ingestion, so books do not need part files. Source readings may intentionally have no CEFR level and are marked level_status: ungraded.

Alice i Eventyrland is a complete Bokmål translation with a provisional independent AI review. It remains ungraded and is not native-editor approved or CEFR-certified. The catalog also includes 26 English source editions marked `translation_status: awaiting_translation`; exclude them from Norwegian reading imports until their translations and reviews are complete.

To import a story, use its HTTPS raw GitHub URL with the app's `reading_ingest` command. Pin that URL to a release commit or tag.

Each story also includes a 512×768 cover derivative in `covers/`. `COVERS.md` lists the source page, license, creator, and image changes; story frontmatter and `catalog.json` expose the corresponding `cover_url` and provenance fields.
