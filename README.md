<p align="center">
  <img src="assets/e-editiones-logo.png" alt="e-editiones" width="280">
</p>

# Open Processing Model (OPM)

*A second, independent implementation of an open standard — bringing the TEI Processing Model to the Python research environment.*

## The challenge

The **TEI Processing Model** is an open standard (TEI Guidelines, Chapter 23.5.4) that describes how TEI-encoded texts are transformed into output formats such as HTML, PDF, or LaTeX. Instead of writing thousands of lines of custom XSLT, editors declare their transformation rules in ODD files using TEI's own vocabulary.

Yet despite being an open standard since 2016, only one complete implementation exists: TEI Publisher, built on the XML database eXist-db. Anyone who wants to use the Processing Model must operate eXist-db — specialised infrastructure that many projects, especially smaller ones, cannot afford to maintain.

Meanwhile Python has become the lingua franca of the Digital Humanities — the language of corpus linguistics, NLP, and machine learning, and of tools like CollateX, spaCy, NLTK, and Jupyter. But there is no way to use the TEI Processing Model in these environments.

> A standard with only one implementation is, in practice, a proprietary format.

## The solution

e-editiones — the Swiss non-profit behind TEI Publisher — proposes two self-contained, independently fundable sub-projects, plus targeted upstream work on the standard itself. Each delivers a usable output on its own; together they form the complete intervention. Funding can start from CHF 30,000 for Sub-project 1 and extend modularly.

### Sub-project 1 — Python implementation of the TEI Processing Model

A lightweight, open-source Python library (`pip install`) that transforms TEI documents according to ODD specifications, without requiring eXist-db. Outputs: **HTML, LaTeX, plain text**. Usable as a library, a command-line tool, or in existing Python workflows — Jupyter notebooks, CI/CD pipelines, serverless deployments.

*Budget: CHF 30,000 (minimum) – CHF 42,000 (full).*

### Sub-project 2 — Abstraction layer in `tei-publisher-lib`

An abstraction layer in the existing core library, decoupling its XQuery core from eXist-db-specific APIs and enabling alternative XQuery engines (BaseX, Saxon) in the future.

*Budget: CHF 24,000 (minimum) – CHF 32,400 (full).*

### Cross-cutting — Direct collaboration with the TEI Technical Council

Contributing into the Council's ongoing work on the next iteration of the Processing Model specification. The independent second implementation systematically surfaces ambiguities, gaps, and de-facto extensions in the Processing Model; these findings are brought back as concrete proposals. Included proportionally in both sub-projects.

### At a glance

| | |
|---|---|
| **Structure** | Two self-contained, independently fundable sub-projects |
| **Entry budget** | From CHF 30,000 (Sub-project 1, minimum) |
| **Full build-out** | Up to CHF 75,000 (both sub-projects, full) |
| **Sponsor** | e-editiones (Swiss non-profit association) |
| **Outputs** | Open-source Python library on PyPI, abstraction layer in `tei-publisher-lib`, contributions to the TEI Technical Council |

## Project team

**Project leads:** Wolfgang Meier (creator of TEI Publisher) and Magdalena Turska (TEI Processing Model co-author, former TEI Technical Council member).

**Steering Committee:** Dr. Helena Bermúdez Sabel (JinnTec, TEI Technical Council), Dr. Anne Diekjobst (Co-President e-editiones, ULB Bonn), Dr. Andreas Kränzle (Co-President e-editiones, Karl Barth Edition), Dr. Andreas Wagner (Max-Planck-Institut für Rechtsgeschichte und Rechtstheorie, Frankfurt).

## How you can support this project

We are seeking support from institutions that share our commitment to open standards and sustainable digital infrastructure for the humanities.

**Partnership levels**

- **Sustaining Partner** (CHF 10,000+) — logo on landing page, acknowledgment in all publications, named in the PyPI package metadata, seat on the Steering Committee.
- **Supporting Partner** (CHF 5,000–9,999) — logo on landing page, acknowledgment in all publications.
- **Contributing Partner** (CHF 1,000–4,999) — name on landing page, acknowledgment in final report.
- **Friend of the Project** (up to CHF 999) — name on landing page.

You can also write a **Letter of Support**, **become a member of e-editiones**, or contribute **in kind** (test data, beta testing, dissemination through your networks). See the prospectus for details.

## Read more

- **[Prospectus (English, 11 May 2026)](prospectus-2026-05-11.pdf)** — full project description and call for partners and supporters
- **Code:** `tei-publisher-py` *(public release forthcoming)*
- **Standard:** [TEI Guidelines, Chapter 23.5.4 — *Specifying Web Output*](https://tei-c.org/release/doc/tei-p5-doc/en/html/TD.html)

## About e-editiones

[e-editiones](https://e-editiones.org) is a Swiss non-profit dedicated to the cooperative development of open-source tools for digital scholarly editions. It coordinates the development of TEI Publisher — the de facto standard for TEI-based publishing in Switzerland — and acts as project sponsor. The [e-editiones project registry](https://www.e-editiones.org/map/) lists over 40 edition projects worldwide that use TEI Publisher.

## Contact

[info@e-editiones.org](mailto:info@e-editiones.org)
