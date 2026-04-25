# ISST — Information-Enhanced Gravity

LaTeX source for *Information-Enhanced Gravity: A Scalar-Tensor Theory Without Dark Matter, Dark Energy, or Cosmological Constant* (S. Brailsford, Lily Labs).

This is a working manuscript. It has not been peer reviewed. The companion site at [lily-labs.co.uk/isst](https://lily-labs.co.uk/isst) presents the theory in plain language; **this repository is the authoritative source**.

## Reading the paper

The compiled PDF is committed to this repository at [`isst_paper.pdf`](./isst_paper.pdf) and is rebuilt automatically on every push by [`.github/workflows/build-pdf.yml`](./.github/workflows/build-pdf.yml). Every revision shows a manuscript ID and date in the footer, so a downloaded copy is never ambiguous about its provenance.

## Building locally

```sh
latexmk -pdf isst_paper.tex
```

Local builds will show `local-build` and today's date in the footer. CI builds inject the short git SHA and commit date instead — see the workflow file for the exact mechanism.

## Layout

- `isst_paper.tex` — main manuscript (compile this)
- `bibliography.bib` — references
- `fig*.pdf`, `fig*.png` — figures
- `version.tex` — generated at build time, gitignored
- `.github/workflows/build-pdf.yml` — CI compile + commit-back

## Citing this work

Until the manuscript is published, cite the repository commit:

> S. Brailsford, *Information-Enhanced Gravity: A Scalar-Tensor Theory Without Dark Matter, Dark Energy, or Cosmological Constant* (manuscript, Lily Labs, YYYY), commit `<short-sha>`. https://github.com/<owner>/<repo>

## Errors and falsifying observations

This work has pre-committed kill conditions. If you find a fatal flaw or a contradicting observation, please open an issue.
