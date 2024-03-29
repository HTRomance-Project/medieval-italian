HTRomance, Medieval Italian corpus of ground-truth for Handwritten Text Recognition and Layout Segmentation
=====================
![characters badge](badges/characters.svg) ![regions badge](badges/regions.svg) ![lines badge](badges/lines.svg) ![files badge](badges/files.svg)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8256728.svg)](https://doi.org/10.5281/zenodo.8256728)

<!-- Custom Zone -->

## Introduction

This ground-truth dataset has been carefully built around the idea of having generic data for building a strong and reliable model for HTR of Italian manuscripts. Each manuscript should have around 10 columns (5 bi-columns pages or 10 pages of single column).

Data follow the Segmonto guidelines.

> [!NOTE]
> The repository contains two XML files per image. The ones suffixed with `.chocomufin.xml` are normalized in order to be compliant with other datasets following the same guidelines. The others are more specific to this repository. We recommend using the normalized documents.

## Credits

- Transcriptions: Rachele Alba, Giorgia Rubin.
- Supervision and manuscript selection: Federic Boschetti, Franz Fischer.
- Project management: Thibault Clérice, Alix Chagué.

<!-- Rien ne doit être modifié manuellement après la balise Start Auto -->

<!-- Start Auto -->

## Transcription guidelines

The transcription guidelines are described in a paper available on [HAL](https://hal-enc.archives-ouvertes.fr/hal-03828353) and published at the Journal for Open Humanities Data. It provides specific details about the selection process, the transcription methods and choices, as well as details about output (mainly the [Generic CREMMA Model for Medieval Manuscripts (Latin and Old French)](https://zenodo.org/record/7234166#.Y7f69afMJhE) for [Kraken](https://kraken.re))

## Data

ALTO and images can be found in the directory data. Each subfolder of data corresponds to a 
single manuscript, identified by its bookshelf.

<!-- BeginTable -->

| Shelfmark                                                        | Folder                                      | Biblissima   | Range   | Type   |   Century | Color   |   Main Zones |   Lines |   Characters | Genre        | Content                            |
|------------------------------------------------------------------|---------------------------------------------|--------------|---------|--------|-----------|---------|--------------|---------|--------------|--------------|------------------------------------|
| [BnF Ita 912](https://gallica.bnf.fr/ark:/12148/btv1b52501692k)  | [🔗](../medieval-italian/data/bnf-ita-912)  |              | 2r-6v   | prose  |        14 | ✓       |            5 |      94 |         1613 | prose        | Cataloghi di prezzi delle merci    |
| [BnF Ita 783](https://gallica.bnf.fr/ark:/12148/btv1b52515037r)  | [🔗](../medieval-italian/data/bnf-ita-783)  |              | 12v-17r | prose  |        14 | ✓       |            5 |     157 |         6398 | prose        | Dandolo, Cronica                   |
| [BnF Ita 434](https://gallica.bnf.fr/ark:/12148/btv1b84363869)   | [🔗](../medieval-italian/data/bnf-ita-434)  |              | 1v-3v   | prose  |        14 | ✓       |            5 |     185 |         8576 | prose        | Marco Polo, Il Milione             |
| [BnF Ita 590](https://gallica.bnf.fr/ark:/12148/btv1b8433319z)   | [🔗](../medieval-italian/data/bnf-ita-590)  |              | 16r-18r | prose  |        14 | ✓       |           10 |     454 |         9377 | poésie+prose | Virgilio, Eneide (volgarizzamento) |
| [BnF Ita 79](https://gallica.bnf.fr/ark:/12148/btv1b52507492w)   | [🔗](../medieval-italian/data/bnf-ita-79)   |              | 54r-56r | vers   |        14 | ✓       |           11 |     423 |        11773 | poésie       | Dante, La divina commedia          |
| [BnF Ita 481](https://gallica.bnf.fr/ark:/12148/btv1b84268148)   | [🔗](../medieval-italian/data/bnf-ita-481)  |              | 41r-43r | prose  |        14 | ✓       |           10 |     512 |        15667 | prose        | Boccaccio, Filocolo                |
| [BnF Ita 594](https://gallica.bnf.fr/ark:/12148/btv1b8433322f)   | [🔗](../medieval-italian/data/bnf-ita-594)  |              | 25r-29v | vers   |        15 | ✓       |            5 |     244 |         5132 | poésie       | El Sinibaldo                       |
| [BnF Ita 70](https://gallica.bnf.fr/ark:/12148/btv1b8426803g)    | [🔗](../medieval-italian/data/bnf-ita-70)   |              | 81r-85v | vers   |        15 | ✓       |            7 |     338 |         7361 | poésie       | Dante, La divina commedia          |
| [BnF Ita 583](https://gallica.bnf.fr/ark:/12148/btv1b84333085)   | [🔗](../medieval-italian/data/bnf-ita-583)  |              | 41r-43r | vers   |        15 | ✓       |           10 |     373 |         9909 | poésie       | Boccaccio, Teseida                 |
| [BnF Ita 1534](https://gallica.bnf.fr/ark:/12148/btv1b52504356m) | [🔗](../medieval-italian/data/bnf-ita-1534) |              | 91-100  | vers   |        16 | ✓       |           10 |     181 |         4179 | poésie       | G.B. Strozzi, Rime                 |
| [BnF Ita 820](https://gallica.bnf.fr/ark:/12148/btv1b52500670h)  | [🔗](../medieval-italian/data/bnf-ita-820)  |              | 2r-6v   | prose  |        16 | ✓       |            5 |     125 |         4680 | prose        | Vita di Cola di Rienzo (et alia)   |

<!-- EndTable -->

## Metrics

<!-- StartMetric -->

### Regions

- DropCapitalZone (192)
- MainZone (83)
- MarginTextZone (30)
- NumberingZone (40)
- GraphicZone (1)
- QuireMarksZone (2)
- RunningTitleZone (5)

### Lines

- DropCapitalLine (244)
- DefaultLine (2814)
- HeadingLine (26)
- InterlinearLine (2)

<!-- EndMetric -->

## Funding

This project was funded by the Bibliothèque nationale de France through the 2022 project calls from
[Datalab](https://www.bnf.fr/fr/bnf-datalab).

## Cite the project

> Clérice, T., Chagué, A., Gille-Levenson, M., Brisville-Fertin, O., Pinche, A., Camps, J., Fischer, F., Boschetti, F., Guadagnini, E., Guilhem Couffignal, G., Canteaut, O., Romary, L., Reboul, M., Perreaux, N., Poibeau, T., Smith, M., Norindr, J., Glaise, A., Navas Farré, M., Bordier, J., Leroy, N., Alba, R., & Rubin, G. *HTRomance* [Data set]. https://htromance-project.github.io/
```
@misc{Clerice_HTRomance,
author = {Clérice, Thibault and Chagué, Alix and Gille-Levenson, Matthias and Brisville-Fertin, Olivier and Pinche, Ariane and Camps, Jean-Baptiste and Fischer, Franz and Boschetti, Federico and Guadagnini, Elisa  and Guilhem Couffignal, Gilles and Canteaut, Olivier and Romary, Laurent and Reboul, Marianne and Perreaux, Nicolas and Poibeau, Thierry and Smith, Marc and Norindr, Jade and Glaise, Anthony and Navas Farré, Marina and Bordier, Julie and Leroy, Noé and Alba, Rachele and Rubin, Giorgia},
title = {{HTRomance}},
url = {https://htromance-project.github.io/}
}
```

## Infrastructure

This project relied on the [CREMMA infrastructure](https://www.dim-map.fr/projets-soutenus/cremma/).


