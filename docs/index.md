# Research study docs

Personal notes from articles and papers, plus longer thesis-style write-ups and synthesis. This site mirrors the repository and is built with [MkDocs](https://www.mkdocs.org/) and [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

## Two use cases

| Use case | Folder | Template | When to use |
|----------|--------|----------|-------------|
| **Paper / article reading** | [Papers](papers/index.md) | [Paper reading template](templates/paper-reading.md) | One source per file: metadata, summary, critique, and follow-ups. |
| **Thesis-style study** | [Studies](studies/index.md) | [Thesis study template](templates/thesis-study.md) | Multi-source or narrative work: literature review, synthesis, arguments, and conclusions. |

The [writing guide](style.md) covers naming, front matter, and Markdown conventions.

## Examples

- [Example paper reading](examples/example-paper-reading.md)
- [Example thesis-style study](examples/example-thesis-study.md)

## Source repository

Content lives in the same Git repo as this site. Edit Markdown under `papers/`, `studies/`, `templates/`, and `examples/` on the default branch; pushing triggers a rebuild if [GitHub Pages](https://pages.github.com/) is configured for GitHub Actions.
