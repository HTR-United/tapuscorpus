Shield: [![CC BY 4.0][cc-by-shield]][cc-by]


# TAPUSCORPUS
## Description
Ground Truth dataset for French typewritten OCR

## Content

**86 pairs of images and PAGE XML files divided into 9 sub-corpus.**


| # | name | nb img | GT for seg | GT for trans |
| --- | :---- | :---: | :---: | :---: |
| 1 | 3vagues_Bordes_nd | (15) | y | y |
| 2 | Cat_MNATP_1962| (14) | n | y |
| 3 | Desnos_Divers_1922-1945 | (14) | y | y |
| 4 | Jardin_Toussaint_nd | (12) | y | y |
| 5 | Journal_Trépond_nd | (9) | y | y |
| 6 | Lettre_Delatre_Foley_nd | (4) | y | y |
| 7 | Parallélisme_Jammes_1929| (6) |y | y | 
| 8 | Poesie_Pau_1962 | (2) | y | y |
| 9 | Rapport_BNF_1984 | (10) | y | y |

- (3): images are blurred (low quality), but readable none the less.


## Annotation system

Undescored words are preceded with `_`such as "<ins>This is an</ins> example" will be transcribed as: "\_This \_is \_an example"

Crossed out words are not rendered:
- words that be read under the stroke are transcribed as if not crossed out
- words that cannot be read under the stroke are transcribed like any portion of text that is not type-written

Any portion of text that is not type-written is transcribed as a series of `~~~` (always 3). There are as many repetition of `~~~` (with a space between each instance) as there are words.


This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
