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

## Documentation site (GitHub Pages)

The repo builds a **Material for MkDocs** site (sidebar, search, mobile-friendly layout) from the [`docs/`](docs/) entry point. Content still lives at the repo root (`papers/`, `studies/`, `templates/`, `examples/`); those folders are linked into `docs/` so you edit files in one place.

**Local preview**

```bash
python3 -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
mkdocs serve
```

Open the URL shown (usually `http://127.0.0.1:8000/`).

**Publish with GitHub Actions**

1. Push this repo to GitHub.
2. **Settings → Pages**: set **Source** to **GitHub Actions** (not “Deploy from a branch”).
3. The workflow [`.github/workflows/docs.yml`](.github/workflows/docs.yml) runs on every push to `main` and deploys the `site/` build.

After the first successful deploy, uncomment and set `site_url` and `repo_url` at the top of [`mkdocs.yml`](mkdocs.yml) so canonical links and the header repository button match your GitHub user and repo name.

**New pages in the sidebar**  
Add each new file under `papers/` or `studies/` to the `nav` section in `mkdocs.yml` (see the existing **Papers** / **Studies** entries).

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
