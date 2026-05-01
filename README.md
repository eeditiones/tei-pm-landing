<p align="center">
  <img src="assets/e-editiones-logo.png" alt="e-editiones" width="280">
</p>

# An Open Implementation of the TEI Processing Model

*A second, independent implementation of an open standard — bringing the TEI Processing Model to the Python research environment.*

## What this project does

Scholarly editions today increasingly need to appear as printed books, websites, PDFs, and searchable data — all from the same source. The **TEI Processing Model**, an open international standard published in 2016, makes this possible by letting editors declare display rules in their data, rather than re-implementing them in custom code for every project.

Yet only one implementation of this standard exists, and it requires a specialized XML database (eXist-db) — a high bar for smaller editions and out of step with the Python-based tooling now standard across the Digital Humanities.

We are building **a second, independent implementation in Python**: a lightweight library, installable with a single command, that brings the Processing Model to the Python research environment. Wherever Python tools are at home — Jupyter notebooks, command-line scripts, CI pipelines — the Processing Model can come along.

## Project goals

The project is structured as two independently fundable sub-projects, plus cross-cutting work on the standard itself.

### Sub-project 1 — Python implementation of the TEI Processing Model

A lightweight, open-source Python library — `tei-publisher-py` — that transforms TEI documents according to ODD specifications, without requiring eXist-db. Distributed via PyPI, usable as a library or as a command-line tool (`teipublisher`) in existing Python workflows: Jupyter notebooks, NLP pipelines, CI/CD, batch processing, headless rendering. Outputs: HTML and Markdown (already in the working prototype), LaTeX and plain-text (in the scope of this project).

*Aims:* lower the entry barrier for editions of any size; bring the Processing Model into the Python ecosystem where most Digital Humanities work happens today.

### Sub-project 2 — Abstraction layer in `tei-publisher-lib`

An abstraction layer in the existing core library, decoupling its XQuery core from eXist-db-specific APIs. With an eXist-db adapter for backward compatibility and a BaseX adapter as a second, working proof-of-concept implementation.

*Aims:* reduce TEI Publisher's dependency on a single XML database; enable alternative XQuery engines (BaseX, Saxon) in the future; make the existing platform more flexible and future-proof.

### Cross-cutting — Specification feedback to the TEI Technical Council

A second, independent implementation surfaces ambiguities and missing details in the specification, and identifies TEI Publisher extensions that should be standardized. Concrete proposals are submitted to the TEI Technical Council for inclusion in the TEI Guidelines.

*Aims:* harden the open standard; ensure ODD portability — the same ODD file should produce equivalent results in both implementations; reduce the standard's dependency on any single implementation.

## Read more

- **[Prospectus (English, 18 April 2026)](prospectus-2026-04-18.pdf)** — full project description and call for institutional support
- **Code:** `tei-publisher-py` *(public release forthcoming)*
- **Standard:** [TEI Guidelines, Chapter 23.5.4 — *Specifying Web Output*](https://tei-c.org/release/doc/tei-p5-doc/en/html/TD.html)

## Supporters

*To be announced.*

## About e-editiones

[e-editiones](https://e-editiones.org) is an international non-profit association based in Switzerland, dedicated to the cooperative development of open-source tools for digital scholarly editions — including TEI Publisher and now its Python implementation.

## Contact

[info@e-editiones.org](mailto:info@e-editiones.org)
