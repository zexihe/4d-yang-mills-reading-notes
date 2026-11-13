# Reading Notes on Four-Dimensional Yang–Mills Theory

Maintained by Zexi He.

These notes are intended for personal study and discussion of the four-dimensional Yang–Mills construction in [OpenAI's Lean proof, OpenAI-YM-20261028](https://github.com/yang-mills-group/OpenAI-YM-20261028). My aim is to develop an account that I can understand and share with the mathematical community.

## Contents and approach

The repository will contain two collections:

- **AI-generated working exposition:** [PDF](4DYM_reading_notes.pdf) · [TeX source](4DYM_reading_notes.tex), a developing account based on the Lean construction and related mathematical expositions.
- **Personal study notes:** my handwritten notes, transcribed, translated and edited into English with AI assistance.

I do not aim for a line-by-line correspondence with Lean. Some notation has been changed to suit my use. AI is also used to expand intermediate calculations and explore possible simplifications. These adaptations require their own justification and do not inherit the verification status of the formal source.

I have no background in the renormalization-group method and have not systematically studied Balaban’s work. A self-contained account is a goal, rather than a description of the present draft.

## AI assistance and review status

The main exposition is substantially AI-generated. I study mainly through questions and answers with AI, asking for explanations of steps I do not understand. I have not read or checked the entire exposition line by line. My study of selected calculations does not constitute a full verification.

These notes have not been mechanically checked against Lean, and I have not locally replayed the original formal proof.

**Current status.** The proof draft has been assembled through its final construction argument, but remains a working exposition subject to correction. It has not undergone an exhaustive independent mathematical review.

The notes do not claim a proof of a positive mass gap.

## Sources

The Lean source used is revision [`3456e5e75cf8d4cd558955a5c7638fba2d68f464`](https://github.com/yang-mills-group/OpenAI-YM-20261028/tree/3456e5e75cf8d4cd558955a5c7638fba2d68f464).

Related sources include the [Yang–Mills informalization project maintained by Scott Armstrong](https://github.com/scottnarmstrong/yang-mills-informalization/tree/1a47ac9007f80d37832291cc12d578874ff6bef9). Borrowed arguments and mathematical results should also be credited where they are used.

The versions cited in the exposition are the [241-page main manuscript](https://github.com/scottnarmstrong/yang-mills-informalization/blob/1a47ac9007f80d37832291cc12d578874ff6bef9/manuscript/main.pdf) and the [595-page detailed notes](https://github.com/scottnarmstrong/yang-mills-informalization/blob/1a47ac9007f80d37832291cc12d578874ff6bef9/pdf/yang-mills-detailed-notes.pdf) at that revision. Page, proposition and equation references refer to those versions.

These are personal reading notes, not an official exposition or an endorsement by OpenAI or the source contributors.

## Building the PDF

The main TeX source is standalone, with its bibliography included. With a LaTeX installation providing XeLaTeX and `latexmk`, run:

```sh
latexmk -xelatex -interaction=nonstopmode -halt-on-error 4DYM_reading_notes.tex
```

## Corrections and updates

Corrections, missing references and alternative explanations are welcome through GitHub Issues. Please identify the document version, section, equation or proposition, and the step that needs justification.

I intend to update the notes as my study progresses, with no fixed schedule for updates or replies. Changes can be followed through the repository’s commit history.
