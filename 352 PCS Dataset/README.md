# 352 PCS Dataset — Pitch-Class Sets Sorted by Roughness

**Francesco Scagliola**  
Coordinator of the PhD Programme in  
*Composizione Musicale Elettroacustica Computazionale, Modelli Algoritmici Generativi e Complessità Computazionale*  
Conservatorio di Musica “Niccolò Piccinni” di Bari

**Version:** 1.0  
**Publication date:** 7 October 2026  
**DOI:** https://doi.org/10.5281/zenodo.23214708

## Description

The **352 PCS Dataset** contains 352 pitch-class sets represented as structured records and ordered according to roughness-related measures.

The dataset was generated using a spectral model based on:

- **Number of harmonics:** 32
- **Base note:** MIDI 60

Each pitch-class set is represented by an integer identifier and an associative record containing pitch content, roughness measures, interval-class information, and parent/child relationships between sets.

The dataset is intended for research in computational music theory, psychoacoustics, algorithmic composition, electroacoustic music, and music computing.

## Dataset structure

Each record contains the following fields:

- `integerNumber` — integer representation of the pitch-class set
- `chord` — pitch-class content
- `rough` — calculated roughness value
- `numIntervalliChord` — number of intervals considered in the chord
- `roughMedia` — mean roughness
- `vettoreIntervallare` — interval-class vector
- `roughVI` — roughness associated with the interval-class vector
- `vettoreIntervallareConUnisono` — interval-class vector including unisons
- `roughVIU` — roughness associated with the interval-class vector including unisons
- `figliChord` — child pitch-class sets
- `figliIntegerNumber` — integer identifiers of child sets
- `padriIntegerNumber` — integer identifiers of parent sets
- `padriChord` — parent pitch-class sets

## Files

The repository contains the dataset and its derived representations in several formats:

- `scrittura01 Associazioni Roughness Dataset.nb`  
  Wolfram Mathematica notebook containing the dataset.

- `scrittura01 Associazioni Roughness Dataset&Code.nb`  
  Wolfram Mathematica notebook containing the dataset and related source code.

- `352_PCS_Dataset_Roughness_H32_MIDI60.json`  
  Machine-readable JSON representation of the complete dataset.

- `352_PCS_Dataset_Roughness_H32_MIDI60.pdf`  
  Human-readable PDF representation of the dataset and graphical outputs.

- `352_PCS_Dataset_Source.zip`  
  Markdown and LaTeX source files together with the `images` directory required to preserve relative figure links.

- `2026_10_07_15_24_59_360midiFile.mid`  
  MIDI material associated with the dataset.

## JSON format

The JSON file provides a software-independent representation of the dataset.

The original ordering of the Wolfram Association is preserved explicitly in the `order` array. Keys in the `dataSet` object are JSON strings corresponding to the original integer keys.

This format allows the dataset to be processed without requiring Wolfram Mathematica.

## Figures and document sources

The Markdown and LaTeX documents reference graphical files using relative paths to the `images` directory.

When using the source package, keep the following structure unchanged:

```text
352_PCS_Dataset_Source/
├── 352_PCS_Dataset_Roughness_H32_MIDI60.md
├── 352_PCS_Dataset_Roughness_H32_MIDI60.tex
└── images/
    └── ...
```

## Repository

GitHub:

https://github.com/FrancescoScagliola/Repository/tree/main/352%20PCS%20Dataset

## DOI

Zenodo:

https://doi.org/10.5281/zenodo.23214708

## Citation

If you use this dataset in research, please cite:

> Scagliola, F. (2026). *352 PCS Dataset: Roughness Measures and Interval-Class Associations* (Version 1.0) [Dataset]. Zenodo. https://doi.org/10.5281/zenodo.23214708

## License

The dataset, metadata, documentation, figures, and other non-code research materials are licensed under the **Creative Commons Attribution 4.0 International License (CC BY 4.0)**.

See:

`LICENSE-DATA.txt`

Source code is licensed under the **GNU General Public License v3.0 (GPL-3.0)**.

See:

`LICENSE-CODE.txt`

## Author

**Francesco Scagliola**  
Conservatorio di Musica “Niccolò Piccinni” di Bari  
Coordinator of the PhD Programme in  
*Composizione Musicale Elettroacustica Computazionale, Modelli Algoritmici Generativi e Complessità Computazionale*