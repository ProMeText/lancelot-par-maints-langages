
![banner](img/lancelot_banner_final_1600x400_clean.png)

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC--BY--NC--SA--4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
[![Paper: CHR 2024](https://img.shields.io/badge/📄_Paper-CHR%202024-blue)](https://ceur-ws.org/Vol-3834/paper104.pdf)

# Across Languages, Lancelot Rides  
*Tracing Lancelot’s journey not only through lands and courts, but through languages, manuscripts, and time.*

> An aligned multilingual corpus of the *Lancelot en prose*, processed with [Aquilign](https://github.com/ProMeText/Aquilign).


## Description

This repository provides training and evaluation data for the study of the multilingual medieval textual tradition of the *Lancelot en prose*, including both manually corrected alignments and automatically generated outputs.

It features a curated selection of witnesses from the *Lancelot en prose*, one of the core cycles of the Arthurian literary corpus. The texts are presented in multiple medieval languages—Old French, Old Spanish (Castilian), and Old Italian—and have been automatically segmented and aligned using the [Aquilign](https://github.com/ProMeText/Aquilign) pipeline, a BERT-based tool for multilingual clause-level alignment of medieval texts.

In addition to alignment outputs, the repository includes manual corrections and evaluation files to support philological analysis and computational validation.

---

## Context and Corpus Description

This project is part of a broader study on **computational multilingual alignment and stemmatological analysis** of medieval texts. The case study focuses on the *Lancelot en prose*, a major prose romance composed anonymously in the early 13th century. With at least 126 surviving manuscript witnesses and numerous translations, the *Lancelot* represents one of the most widespread and complex textual traditions of medieval Europe.

This corpus includes aligned segments from the Medieval Romance tradition—specifically:
- **French (source)**,
- **Castilian**, and
- **Italian**.

Due to the fragmentary and unstable nature of the textual transmission, only **comparable segments** from selected witnesses were retained. Alignment is performed at the **clause (“sentence”) level**, preceded by a segmentation step using a custom-trained model. The aligned outputs are then used for **variant classification** and **stemmatological exploration**.

---

## Alignment Tool
The corpus was processed using [Aquilign](http://github.com/ProMeText/Aquilign), a multilingual alignment tool developed by the [ProMeText](https://github.com/ProMeText) team.

 - **Segmentation**: Performed at the clause level using custom token classification models trained on historical data.  
  For detailed information about the segmentation guidelines, training data, and language coverage, see the [Multilingual Segmentation Dataset](https://github.com/carolisteia/multilingual-segmentation-dataset) repository, particularly its [`/docs/`](https://github.com/carolisteia/multilingual-segmentation-dataset/tree/main/docs) folder.

- **Alignment**: Based on contextual embeddings generated with [LaBSE](https://github.com/google-research/bert/blob/master/multilingual.md) and processed through [Bertalign](https://github.com/bfsujason/bertalign), enabling cross-lingual comparision between the different textual witnesses.

- **Languages**:  Medieval French, Castilian, and Italian


---

##  Visualization

Example of multilingual alignment table:
👉 [View aligned chapter](https://github.com/carolisteia/lancelot-par-maints-langages/blob/main/segmentation_alignment_results/outputs/lancelot_1_bert_new/final_result.html)


## Contributing to the Project

Contributions to the project are highly encouraged, whether they be additional data, bug fixes, or enhancements to the analysis scripts. To contribute:

1. **Fork the Repository** – Start by forking the repository and cloning it locally.  
2. **Create a Branch** – Make your changes in a new branch named after the feature or fix.  
3. **Submit a Pull Request** – After pushing your changes to your fork, open a pull request for discussion and review.


## Citation
If you use the corpus or refer to the alignment methodology, please cite:

> Gille Levenson, M., Ing, L., & Camps, J.-B. (2024).  
> *Textual Transmission without Borders: Multiple Multilingual Alignment and Stemmatology of the "Lancelot en prose" (Medieval French, Castilian, Italian).*  
> In W. Haverals, M. Koolen, & L. Thompson (Eds.), *Proceedings of the Computational Humanities Research Conference 2024* (Vol. 3834, pp. 65–92). CEUR.  
> [https://ceur-ws.org/Vol-3834/#paper104](https://ceur-ws.org/Vol-3834/#paper104)

```bibtex
@inproceedings{gillelevenson_TextualTransmissionBorders_2024a,
  title = {Textual {{Transmission}} without {{Borders}}: {{Multiple Multilingual Alignment}} and {{Stemmatology}} of the ``{{Lancelot}} En Prose'' ({{Medieval French}}, {{Castilian}}, {{Italian}})},
  shorttitle = {Textual {{Transmission}} without {{Borders}}},
  booktitle = {Proceedings of the {{Computational Humanities}}   {{Research Conference}} 2024},
  author = {Gille Levenson, Matthias and Ing, Lucence and Camps, Jean-Baptiste},
  editor = {Haverals, Wouter and Koolen, Marijn and Thompson, Laure},
  date = {2024},
  series = {{{CEUR Workshop Proceedings}}},
  volume = {3834},
  pages = {65--92},
  publisher = {CEUR},
  location = {Aarhus, Denmark},
  issn = {1613-0073},
  url = {https://ceur-ws.org/Vol-3834/#paper104},
  urldate = {2024-12-09},
  eventtitle = {Computational {{Humanities Research}} 2024},
  langid = {english},
  file = {/home/mgl/Bureau/Travail/Bibliotheque_zoteros/storage/CIH7IAHV/Levenson et al. - 2024 - Textual Transmission without Borders Multiple Multilingual Alignment and Stemmatology of the ``Lanc.pdf}
}
```


## Funding

This work benefited from national funding managed by the **Agence Nationale de la Recherche** under the *Investissements d'avenir* programme with the reference **ANR-21-ESRE-0005 (Biblissima+)**.

> Ce travail a bénéficié d'une aide de l’État gérée par l’**Agence Nationale de la Recherche** au titre du programme d’**Investissements d’avenir** portant la référence **ANR-21-ESRE-0005 (Biblissima+)**.

<p align="center">
  <img src="https://github.com/user-attachments/assets/915c871f-fbaa-45ea-8334-2bf3dde8252d" alt="Biblissima+ Logo" width="600"/>
</p>

## Licensing

This project is licensed under the [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) license.  
This license allows users to adapt, remix, and build upon the work for non-commercial purposes, provided that they credit the original authors and share any derivative works under the same license.

