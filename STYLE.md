# Writing style and conventions

These rules keep `papers/` and `studies/` consistent and easy to skim in GitHub or any Markdown viewer.

## Shared rules

- **YAML front matter** at the top of every document (between `---` lines). Use the fields defined in each template; leave unknown values empty or omit optional keys.
- **Filenames**
  - Papers: `YYYY-familyname-or-firstauthor-keyword-slug.md` (e.g. `2024-zhang-off-policy-rl.md`). Use lowercase and hyphens.
  - Studies: `topic-or-chapter-slug.md` or `YYYY-topic-slug.md` if versioning by year helps.
- **Headings**: use `##` / `###` only inside the body (title comes from front matter `title`).
- **Citations**: prefer DOI or stable URL in front matter; in the body use inline links or a short reference list at the end.
- **Figures**: store under `papers/assets/<slug>/` or `studies/assets/<slug>/` and link with relative paths, e.g. `![caption](assets/my-note/fig1.png)`.
- **Tone**: papers = concise and source-bound; studies = you may argue, compare sources, and state open questions explicitly.

## Use case 1 — Paper reading (`papers/`)

- One primary source per file unless you are explicitly comparing two papers in a single reading session (then list both in `sources`).
- Aim for **scannable** sections: short paragraphs, bullet lists where they help.
- Always capture **limitations** and **what you would do next** (experiments, papers to read).

## Use case 2 — Thesis-style study (`studies/`)

- Prefer a clear **through-line** (one research question or thesis statement).
- **Synthesis** sections should tie multiple sources together, not summarize them one-by-one only.
- Mark **status** in front matter (`draft`, `review`, `stable`) so long documents evolve safely.
