# hire-your-mck

**Brief it like a partner. Get the deck in minutes.**

A Claude Skill that turns your research, or just the decision you need to make, into a
McKinsey-style PowerPoint deck. It hands you two files:

- `<name>.pptx`: an editable deck with a storyline that holds together, an action title on every
  slide, and native PowerPoint charts you can edit
- `<name>-sources.xlsx`: a source workbook, one sheet per slide, with the value, source, URL and
  a verbatim excerpt for every number, and a live Excel formula for anything calculated

It never invents a number. A number without a source shows as "?" with a note on the data needed.

## How to use it

Brief it in plain words, for example:

> Our CEO has to decide whether to launch an AI package for our small-business customers.
> Build the deck from public data.

It asks a few multiple-choice questions (audience, decision, material, look), shows you the
storyline for approval, finds and sources the data slide by slide, checks the deck against its
rules, and renders the files. It can also build a storyline-only "ghost deck", a single slide, or a
deep 30–60 slide deck worked through as a problem (problem statement, issue tree, a section per branch).

## Setup

The skill renders with the [`hire-your-mck`](https://pypi.org/project/hire-your-mck/) Python package, run through
[`uv`](https://docs.astral.sh/uv/): `uvx hire-your-mck` downloads it on first use. Without `uv`, run
`pip install hire-your-mck` (Python 3.9 or later). Nothing else to configure.

Source code, examples and the rules behind the slides:
[github.com/brianlee0113/hire-your-mck](https://github.com/brianlee0113/hire-your-mck).

MIT licensed. Not affiliated with or endorsed by McKinsey & Company.
