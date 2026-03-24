# Artifacts

This repository contains generated novel artifacts produced by the Autofiction project for the novels published on [autofiction.ai](https://autofiction.ai).

The companion pipeline repository that contains the code used to generate and revise these novels is [AutoFiction-AI/autofiction](https://github.com/AutoFiction-AI/autofiction).

## Structure

The repository root is intentionally compact:

- `README.md`: overview of the archive
- `LICENSE`: usage terms for the artifact corpus
- `books/`: one subdirectory per exported book

Each directory under `books/` is a single exported book.

Book directories preserve the structured outputs of the generation pipeline. Not every book contains every artifact type, but most books include a substantial subset of the following:

- `FINAL_NOVEL.md`: the canonical top-level manuscript for that book
- `generation_metadata.json`: normalized metadata about the exported generation run
- `input/`: premise and other seeded run inputs
- `outline/`: title, outline, chapter specs, style bible, continuity sheet, and related planning files
- `chapters/`: chapter-by-chapter manuscript files
- `context/`: cycle context packs and supporting continuity context
- `reviews/`: chapter reviews, full-book review artifacts, and cross-chapter audit artifacts
- `findings/`: aggregated findings produced from review stages
- `gate/`: per-cycle gate decisions and unresolved-finding summaries
- `packets/`: per-chapter revision packets built from aggregated findings
- `revisions/`: per-cycle revision reports and pass outputs
- `snapshots/`: cycle-local compiled manuscripts, including pre-revision and post-revision snapshots
- `reports/`: final reports, validation summaries, and related export metadata
- `premise/`: alternate premise exports preserved for some books
- `manual_rescue/`: rescue artifacts for a small number of books that required manual intervention
- `posthoc_revision/`: canonical posthoc editorial provenance for books whose shipped text was modified in a posthoc pass

## Posthoc Revision Folders

Some books include a `posthoc_revision/` directory. These folders preserve the canonical structured artifacts for the posthoc pass that produced the shipped text, including:

- `FINAL_NOVEL.posthoc_revision.md`
- structured review and audit JSON artifacts
- revision packets and revision reports
- a short provenance note

Raw job logs (i.e., with every prompt, reasoning trace, and output provided by the model) are intentionally omitted from this repository to keep the artifact archive readable and lightweight. Please email <support@autofiction.ai> if you'd like access to any of these logs!

## License

Unless otherwise noted, the contents of this repository are licensed under the Creative Commons Attribution-NonCommercial 4.0 International license. See [LICENSE](./LICENSE).
