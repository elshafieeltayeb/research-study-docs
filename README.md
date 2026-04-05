# Research study docs

Personal repository for structured notes from articles and papers, plus longer thesis-style write-ups and synthesis.

## Two use cases

| Use case | Folder | Template | When to use |
|----------|--------|----------|-------------|
| **Paper / article reading** | [`papers/`](papers/) | [`templates/paper-reading.md`](templates/paper-reading.md) | One source per file: fast capture after reading—metadata, summary, critique, and follow-ups. |
| **Thesis-style study** | [`studies/`](studies/) | [`templates/thesis-study.md`](templates/thesis-study.md) | Multi-source or narrative work: literature review sections, themed synthesis, arguments, and conclusions. |

See [`STYLE.md`](STYLE.md) for naming, front matter, and Markdown conventions shared by both.

## Quick start

1. Copy the template that matches your goal into the right folder.
2. Rename using the convention in `STYLE.md` (e.g. `papers/2026-smith-rl-for-uavs.md`).
3. Fill YAML front matter first so lists and search stay consistent.

Examples live in [`examples/`](examples/).

## Publish to GitHub

The project is already a Git repository with an initial commit. Create an **empty** repository on GitHub (no README, no license), then:

```bash
cd /Users/elshafieeltayeb/Documents/elshafie/projects/research-study-docs
git remote add origin git@github.com:YOUR_USERNAME/research-study-docs.git
git push -u origin main
```

Replace `YOUR_USERNAME` and the repo name if yours differs. For HTTPS: `https://github.com/YOUR_USERNAME/research-study-docs.git`.

If you use [GitHub CLI](https://cli.github.com/) after `gh auth login`, you can run `gh repo create research-study-docs --private --source=. --remote=origin --push` from this directory instead.

## License

Private notes by default. Add a `LICENSE` if you intend to publish the repo.
