# Reading Notes on Four-Dimensional Yang–Mills Theory

Maintained by Zexi He.

These notes are intended for personal study and discussion of the four-dimensional Yang–Mills construction in [OpenAI's Lean proof, OpenAI-YM-20261028](https://github.com/yang-mills-group/OpenAI-YM-20261028). My aim is to develop an account that I can understand and share with the mathematical community.

## Contents and approach

The repository contains two collections:

- **AI-generated working exposition:** [PDF](4DYM_reading_notes.pdf) · [TeX source](4DYM_reading_notes.tex), a developing account based on the Lean construction and related mathematical expositions.
- **Personal study notes:** [PDF](notes/YM4_study_notes.pdf) · [TeX source](notes/YM4_study_notes.tex), developed from my handwritten notes and transcribed, translated and edited into English with AI assistance. The 15 November 2026 installment covers Wilson measures, exact blocking, tree gauge, Gaussian normalization, the central logarithmic estimate, and conditional small-chart and plaquette-small tail bounds. It also includes a summary of exact sector reassembly and the complementary good–bad tail split. The model-dependent inputs and the remaining large-plaquette contribution are identified explicitly.

I do not aim for a line-by-line correspondence with Lean. Some notation has been changed to suit my use. AI is also used to expand intermediate calculations and explore possible simplifications. These adaptations require their own justification and do not inherit the verification status of the formal source.

I have no background in the renormalization-group method and have not systematically studied Balaban’s work. A self-contained account is a goal, rather than a description of the present draft.

## AI assistance and review status

The main exposition is substantially AI-generated. I study mainly through questions and answers with AI, asking for explanations of steps I do not understand. I have not read or checked the entire exposition line by line. My study of selected calculations does not constitute a full verification.

These notes have not been mechanically checked against Lean, and I have not locally replayed the original formal proof.

**Current status.** The proof draft has been assembled through its final construction argument, but remains a working exposition subject to correction. It has not undergone an exhaustive independent mathematical review.

The main exposition was updated on 15 November 2026 from the manuscript revision of 15 November 2026.

The notes do not claim a proof of a positive mass gap.

## Sources

The formal source is OpenAI's Lean construction, revision [`3456e5e75cf8d4cd558955a5c7638fba2d68f464`](https://github.com/yang-mills-group/OpenAI-YM-20261028/tree/3456e5e75cf8d4cd558955a5c7638fba2d68f464).

The exposition also draws on the [Yang–Mills informalization project maintained by Scott Armstrong](https://github.com/scottnarmstrong/yang-mills-informalization) and [Humanise Yang–Mills, maintained by Martin Hairer](https://github.com/hairer/humanise-yang-mills). The fixed versions used are:

| Material | Version used | Pinned source |
| --- | --- | --- |
| Armstrong project: main manuscript | 11 November 2026, 241 pages | [PDF](https://github.com/scottnarmstrong/yang-mills-informalization/blob/1a47ac9007f80d37832291cc12d578874ff6bef9/manuscript/main.pdf) |
| Armstrong project: detailed notes | 11 November 2026, 595 pages | [PDF](https://github.com/scottnarmstrong/yang-mills-informalization/blob/1a47ac9007f80d37832291cc12d578874ff6bef9/pdf/yang-mills-detailed-notes.pdf) |
| Armstrong project: third draft | 13 November 2026, 278 pages | [PDF](https://github.com/scottnarmstrong/yang-mills-informalization/blob/daf1db452866dd773b17aa955d534e56196a4efc/manuscript/main.pdf) |
| Hairer project: working existence manuscript | Source snapshot of 14 November 2026, locally compiled to 1028 pages | [TeX source](https://github.com/hairer/humanise-yang-mills/blob/25838a29809d35e83138a2091a4037cd8238734b/manuscript/existence.tex) |

Section, equation and page locators refer to these versions. For the Hairer working snapshot, the bundled `manuscript/existence.pdf` is an older 872-page PDF; the page locators in these notes refer to the 1028-page PDF compiled locally from the pinned source.

The Hairer material is used for the fixed-coupling auxiliary history (Section 167), the organization of complete marked products and their common normalization (Section 171), and normalized Maxwell and Kelvin responses (Section 199). The Armstrong expositions guide the blocking, local integration, Gaussian comparisons and continuum construction. Specific borrowed arguments and mathematical results are credited where they are used, with precise locators in the bibliography.

These expository sources are working drafts. Adaptations in the present notes require their own justification. These are personal reading notes, not an official exposition or an endorsement by OpenAI or the source contributors.

## Building the PDF

The main TeX source is standalone, with its bibliography included. With a LaTeX installation providing XeLaTeX and `latexmk`, run:

```sh
latexmk -xelatex -interaction=nonstopmode -halt-on-error 4DYM_reading_notes.tex
```

## Corrections and updates

Corrections, missing references and alternative explanations are welcome through GitHub Issues. Please identify the document version, section, equation or proposition, and the step that needs justification.

I intend to update the notes as my study progresses, with no fixed schedule for updates or replies. Changes can be followed through the repository’s commit history.
