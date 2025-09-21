# 🧬 Protein Synthesis Simulator — Python Edition

Welcome to the Protein Synthesis Simulator: a tiny, playful Python project that models the central dogma of molecular biology — from DNA to mRNA to protein. It's perfect for demos, teaching, or just geeking out about codons and amino acids. 🚀

## What it does

- Generates random DNA sequences (with a start codon and a stop codon). 🧩
- Transcribes DNA → mRNA by replacing T with U. ✍️
- Translates mRNA → protein using a simple ribosome model and a codon table. 🔬

## Project structure

- `DNA_Generator.py` — builds random DNA sequences (uses NumPy).
- `ADN.py` — `ADN` class: stores DNA and computes the complementary strand.
- `ARN.py` — `ARN` class: creates mRNA from an `ADN` instance.
- `Ribosoma.py` — `Ribosoma` class: translates mRNA codons into amino acids.
- `Main.py` — example runner that wires everything together and prints results.

## Requirements

- Python 3.7+
- NumPy (used by `DNA_Generator.py`)

Quick install:

```bash
python -m pip install --user numpy
```

Optionally create a virtual environment first:

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install numpy
```

## How to run

Run the main script to generate and translate several DNA sequences:

```bash
python Main.py
```

Note: The repository contains `Main.py` (capital M). If you prefer `main.py`, rename the file or update the README accordingly.

## Example output

You should see blocks like:

- ADN: ATG...TAA
- ARNm: AUG...UAA
- Protein: ['Met', 'Ala', 'Stop']

(Proteins are shown as a list of 3-letter amino acid codes until a stop codon is encountered.)

## Ideas & enhancements (pull requests welcome!) ✨

- Add a `requirements.txt` and a small CLI to control how many sequences to generate.
- Add unit tests (pytest) covering transcription and translation.
- Improve sequence validation (handle incomplete codons, ambiguous bases, etc.).
- Add visualization: colorized codon breakdown, peptide length histograms, etc.

## Credits

Authors: Adrián Perera Moreno & Álvaro Juan Travieso García

Built with ❤️ for education and fun.

