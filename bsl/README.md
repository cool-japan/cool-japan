# The Business Source License at COOLJAPAN

COOLJAPAN OU licenses some of its works under the Business Source License 1.1
(SPDX `BUSL-1.1`): their source is published, non-production use is free, and
production use needs a sponsorship until the Change Date, when the work comes
under the Apache License, Version 2.0. The Licensor regards publishing
software that depends on such a work, in a public repository or on a package
registry, as production use, whether or not that software is commercial.

This directory holds the text that those works share. It is not a licence
itself. Each work ships its own `LICENSE` and `LICENSING.md`, and the
`LICENSE` that a version of a work ships with is what governs that version.

| File | Becomes |
|---|---|
| [`LICENSE.template`](LICENSE.template) | The work's `LICENSE`: the Parameters, with the Additional Use Grant, then the Business Source License 1.1 as MariaDB publishes it |
| [`LICENSING.template.md`](LICENSING.template.md) | The work's `LICENSING.md`: a plain-language summary of what the licence allows, with the sponsorship programme that the `LICENSE` refers to |

The text outside the `{{SLOTS}}` is the same in every work. It was taken from
cargo-formal's `LICENSE` and `LICENSING.md` on 2026-11-13: filling the slots
with cargo-formal's values gives those two files byte for byte.

## What every work shares

- **Licensor:** COOLJAPAN OU (Team KitaSan).
- **Change License:** the Apache License, Version 2.0.
- **Change Date:** `(2030 + major)-01-01`, where major is the first number of
  the version: 2030-01-01 for 0.x, 2031-01-01 for 1.x, 2032-01-01 for 2.x.
  The Business Source License also changes each version on the fourth
  anniversary of its first publication when that comes first.
- **The sponsorship levels** of paragraph (1) of the Additional Use Grant:
  - USD 1,500 per month or more for one work covers that work alone.
  - USD 4,500 per month or more covers up to five works, those the sponsor
    names to the Licensor in writing.
  - USD 12,000 per month or more covers every work under the Business Source
    License.

  A sponsorship covers the individual or the legal entity that holds it, and
  a legal entity's employees and the contractors working for it.
- **Paragraphs (2), (5) and (6)** of the Additional Use Grant: the use that
  needs no sponsorship, the Licensor's own projects, and no further
  restriction. The use that needs no sponsorship does not include publishing
  software that depends on the work.
- **Paragraph (3) (b):** the Licensor regards as production use publishing
  software that depends on the work, whether or not for a fee. Software
  depends on the work when it names the work, or a package built from it, as
  a dependency; it is published when it, or its source, is made available to
  others, for example in a public repository on GitHub or on crates.io. The
  paragraph does not limit the right to copy and redistribute the work
  itself, which the Business Source License grants and lets no Additional Use
  Grant restrict (its covenant 2). This is the owner's decision of
  2026-11-13: being able to download the source is free, while running it in
  production or making a published project depend on it is not.
- **The Business Source License 1.1** after the Parameters, word for word. Its
  covenants allow the Licensor to set the Parameters and to change nothing
  else.

## The slots

The slot names are in capitals between double braces. A slot that appears
more than once takes the same value each time.

### `LICENSE.template`

| Slot | What it holds | cargo-formal's value, in short |
|---|---|---|
| `{{LICENSED_WORK}}` | The versions and the crates that the `LICENSE` covers, and the year of the copyright notice. A work that distributes material under a licence of its own adds the "Licensed separately" paragraph, which points at `THIRD-PARTY-NOTICES.md`. | "cargo-formal 0.1, that is, version 0.1.0 and every later 0.1.x version: the crates … The Licensed Work is (c) 2026 COOLJAPAN OU (Team KitaSan)", then the crates and directories licensed separately |
| `{{PRODUCTION_USE}}` | The rest of (a) in paragraph (3), after "that is,", as one clause: what commercial use of this work consists of | Running the tool on commercially developed software, continuous integration included |
| `{{PRODUCTION_USE_MORE}}` | Sentences that close paragraph (3), after its common text, each starting with a space; or nothing. They say when the work's use counts as production use rather than evaluation | A verification tool's use as a CI job or a release gate counts as production use, however it is described |
| `{{OUTPUT}}` | The list of what the work produces when it is run, in paragraph (4) | Reports, verdicts, counterexample tests, harness scaffolds, baselines, solver scripts, certificates, proof exports, and code it emits into your project |
| `{{CHANGE_DATE}}` | The Change Date, by the rule above | 2030-01-01 |

### `LICENSING.template.md`

| Slot | What it holds | cargo-formal's value, in short |
|---|---|---|
| `{{NAME}}` | The work's name, formatted as the page writes it | `` `cargo-formal` `` |
| `{{KIND}}` | The noun the page uses for the work | tool |
| `{{IN_SHORT_PRODUCTION}}` | One sentence on what production use is, ending in a full stop | Running it on commercially developed software, continuous integration included |
| `{{IN_SHORT_MORE}}` | Any further bullets of "In short", or nothing | The tool's output is yours; the crates that are Apache-2.0 |
| `{{CHANGE_DATE}}` | As in `LICENSE` | 2030-01-01 |
| `{{BSL_PARTS}}` | The table cell for what is under `BUSL-1.1` | The ten tool crates, the documentation and the other files of the repository |
| `{{OTHER_ROWS}}` | Further rows of the table, or nothing. A work that distributes material under a licence of its own lists it here in a "Material written by others" row. | The Apache-2.0 crates and directories, and material written by others |
| `{{PARTS_NOTE}}` | A paragraph about those rows, or nothing | Why `oxiformal` is Apache-2.0 |
| `{{EVALUATION}}` | What trying the work means | "trying it, on your own code too," |
| `{{ADOPTION}}` | When the work counts as adopted. Keep it in step with `{{PRODUCTION_USE}}` of `LICENSE`. | A standing part of how commercial software is developed, released or operated |
| `{{PRODUCTION_USE_DETAIL}}` | The rest of the first paragraph of "What needs a sponsorship", in step with `{{PRODUCTION_USE}}` | Running `cargo formal` on commercially developed software, in CI or by a developer at work |
| `{{PAGE_URL}}` | The Licensor's page for the work. It lists the ways to take out a sponsorship and nothing else. For every other work it is `https://cooljapan.tech/bsl/<work>/`, `<work>` being the name of its repository: the page must be live before the work's first release under the licence. | https://cooljapan.tech/cargo-formal/ |
| `{{EARLIER_CHANGE}}` | Nothing for 0.x. From 1.x on, a paragraph on the four-year limit: "A version first published less than four years before {{CHANGE_DATE}} comes under the Apache License, Version 2.0 earlier, on the fourth anniversary of its first publication, as the `LICENSE` file says." | Nothing |
| `{{OUTPUT_SECTION}}` | A section saying that what the work produces is yours, in step with paragraph (4), or nothing | "What the tool writes is yours" |
| `{{RELEASE}}` | What a release consists of, and which packages carry `LICENSING.md`. A work with Python or npm packages names them too. | The crates on crates.io and nothing else; the ten tool crates carry this page |
| `{{THIRD_PARTY_SECTION}}` | A section that points at `THIRD-PARTY-NOTICES.md`, or nothing | "Material written by others" |

## Filling in

1. Copy the two templates into the work's repository as `LICENSE` and
   `LICENSING.md`. The package of every crate carries both: cargo-formal's
   crates link to the files at the root of the repository.
2. Fill every slot. When a slot that has a line of its own is left empty,
   delete that line, and also one of the blank lines around it if both are
   blank.
3. Re-wrap what you filled in as the template wraps it. In `LICENSE`, the text
   of the Parameters starts at column 23 and lines are at most 79 characters
   long.
4. Check that no `{{` is left in either file.
5. Set `license = "BUSL-1.1"` in the workspace `Cargo.toml`, for every crate.
6. Material that others wrote keeps its own licence. List it in
   `THIRD-PARTY-NOTICES.md`, and keep its own licence files.

## Changing the common text

Change the text here first, then the copy in every work, so that the works do
not drift apart. A change applies to the versions released after it. A
version that is already released keeps the `LICENSE` it was released with,
because the Business Source License applies to each version separately.
