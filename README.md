Shield: [![CC BY 4.0][cc-by-shield]][cc-by]


# TAPUSCORPUS
## Description
Ground Truth dataset for French typewritten OCR

## Content

**86 pairs of images and PAGE XML files divided into 9 sub-corpus.**


| # | name | nb of images | GT for segmenter? | GT for recognizer? | link(s) to source images | 
| --- | :---- | :---: | :---: | :---: | ---: | 
| 1 | 3vagues_Bordes_nd | (15) | y | y | https://gallica.bnf.fr/ark:/12148/btv1b52502601r/manifest.json |
| 2 | Cat_MNATP_1962| (14) | n | y | https://www.siv.archives-nationales.culture.gouv.fr/siv/UD/FRAN_IR_050603/c-2cfmj84sh--fdjfx0b91tk6 |
| 3 | Desnos_Divers_1922-1945 | (14) | y | y | http://bljd.sorbonne.fr/ark:/naan/a011441804309XrO1fa/e3ff656f45 , http://bljd.sorbonne.fr/ark:/naan/a011441804309Dy4ooR/8f9020bc6e , http://bljd.sorbonne.fr/ark:/naan/a01144180430809P21l/036952bd71 , http://bljd.sorbonne.fr/ark:/naan/a0114418043093CzACj/ae2ff446cd |
| 4 | Jardin_Toussaint_nd | (12) | y | y | https://gallica.bnf.fr/ark:/12148/btv1b10581912k/manifest.json |
| 5 | Journal_Trépond_nd | (9) | y | y | https://www.siv.archives-nationales.culture.gouv.fr/siv/UD/FRAN_IR_050082/c-65dxt4cy4--yqhpaasluvz1 |
| 6 | Lettre_Delatre_Foley_nd | (4) | y | y | https://gallica.bnf.fr/ark:/12148/btv1b525062185/manifest.json |
| 7 | Parallélisme_Jammes_1929| (6) |y | y | https://gallica.bnf.fr/ark:/12148/btv1b10583038c/manifest.json |
| 8 | Poesie_Pau_1962 | (2) | y | y | https://gallica.bnf.fr/ark:/12148/btv1b10583138r/manifest.json |
| 9 | Rapport_BNF_1984 | (10) | y | y | https://gallica.bnf.fr/ark:/12148/btv1b53097347b/manifest.json |

- (3): images are blurred (low quality), but readable none the less.


## Annotation system

Undescored words are preceded with `_`such as "<ins>This is an</ins> example" will be transcribed as: "\_This \_is \_an example".

Portions of text that are superscripted are preceded with `^` such as "1<sup>er</sup>" will be transcribed as "1^er". If several words are superscripted, each word starts with a "^".

Crossed out words are not rendered:
- words that be read under the stroke are transcribed as if not crossed out;
- words that cannot be read under the stroke are transcribed like any portion of text that is not type-written.

Any portion of text that is not type-written is transcribed as a series of `~~~` (always 3). There are as many repetition of `~~~` (with a space between each instance) as there are words.


## Citation

This dataset was built by Alix Chagué (@alix-tz).

### How to cite

This dataset was built and is maintained by Alix Chagué (@alix-tz). The original works and their digitization are all copyright-free, but properly annotating a corpus takes time and is a task that should be recognized. If you use any item from this corpus of ground truth, cite the dataset using the following information:

```
name: "Tapuscorpus"
url: 'https://github.com/HTR-United/tapuscorpus'
author: 'Alix Chagué'
month: 'janv'
year: '2021'
version: '{any version}'
description: 'Ground Truth dataset for French typewritten OCR (20th century documents)'
language: French
time: 1900-1999
hands: 12
license:
    - {name: 'CC-BY 4.0', url: 'https://creativecommons.org/licenses/by/4.0/'}
format: PAGE-XML
volume:
    - {count: "86", metric: pages}
```


This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
