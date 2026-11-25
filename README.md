# JCSS Workshop "Societal Preferences on Risk Acceptance" – Waterloo, 21–22 October 2026

Documentation of the workshop as a Jupyter Book, in the same format as the
[2023 Trondheim workshop](https://github.com/JCSS-PMC/2023_Risk_Acc_WS).

## Contents

- `intro.md` – title page, context, how the documentation was produced
- `programme.md` – programme as held, with links to the presentation pages
- `session0.md`, `s1_*.md`, `s2_discussion.md`, `s3_*.md`, `s4_*.md`, `s5_discussion.md` – one page per
  presentation (slides, summary, discussion) and per discussion session
- `conclusions.md` – draft conclusions
- `slides/` – presentation files (PDF; Goda also as PPTX)
- `JCSS_Workshop_Waterloo_Programme_2026.pdf` – the programme as distributed

## Building

```
pip install -r requirements.txt      # jupyter-book < 2
jupyter-book build .
open _build/html/index.html
```

Publishing works as for the 2023 book: push `main`, then publish `_build/html` to the `gh-pages`
branch (e.g. with `ghp-import -n -p -f _build/html`).

## Editing

The text lives in the Markdown files (`*.md`); edit those, then rebuild the HTML with
`jupyter-book build .` (or ask for a rebuild). The HTML in `_build/html` is generated and
should not be edited by hand.
