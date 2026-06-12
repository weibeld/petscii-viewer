# PETSCII Viewer

## Idea

An interactive application for visualsing the [PETSCII character set](https://en.wikipedia.org/wiki/PETSCII) with a focus on the associated Commodore C64 key combinations to select the characters.

Inspired by the [PETSCII Reference](https://style64.org/petscii/) application from <https://style64.org/>.

## Initial Exploration

The [`style64-org-petscii`](#style64-org-petscii) directory contains a modified version of the [PETSCII Reference](https://style64.org/petscii/) app. The introduced changes include:

1. When clicking on a character, also highlight all characters that are selected by including the same physical base key
   - For example, when selecting the character _A_, also highlight the characters with the key combinations _Shift-A_, _CBM-A_, and _Control->_
   - Conversely, when selecting, for example, the character with the key combination _Shift-A_, also highlight the characters with key combinations _CBM-A_, _Control-A_, and just _A_
2. Add an interactive legend for key combination types (_Shift-*_, _CBM-*_, _Control-*_ key combinations and just the bare key itself)
  - For example, when clicking on the _Shift-*_ legend item, highlight all characters that have a key combination that includes the _Shift_ key
  - Also display the count of characters in each key combination group when clicking on a legend item

The code of the original PETSCII Reference app has been obtained with `wget --mirror` and the changes have been implemented by vibe coding with Gemini CLI.

## Resources

| URL | Description |
|:----|:------------|
| <https://style64.org/> | Various Commodore C64 related tools including the interactive [PETSCII Reference](https://style64.org/petscii/) and a [C64 True Type (TTF) Font](https://style64.org/c64-truetype) |
| <https://www.pagetable.com/c64ref/charset/> | Similar app to the [PETSCII Reference](https://style64.org/petscii/) app on <https://style64.org/petscii>, additionally includes entire PETSCII character set in table form, code in the [mist64/c64ref/](https://github.com/mist64/c64ref/tree/main/src/charset) GitHub repository |
| <https://github.com/mist64/c64ref> | Extensive collection of Commodore C64 reference material |
| <https://sta.c64.org/cbmdocs.html> | Misceallaneous collection of Commodore C64 notes and materials, for example, see [Commodore 64 PETSCII codes](https://sta.c64.org/cbm64pet.html) and [Commodore 64 PETSCII codes (with key combinations)](https://sta.c64.org/cbm64petkey.html) |
| <https://www.aivosto.com/articles/petscii.pdf> | Overview of all variants of the PETSCII character sets |
