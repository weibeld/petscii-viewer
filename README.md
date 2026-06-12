# PETSCII Viewer

## Idea

An interactive application for visualsing the PETSCII character encoding system with a focus on the associated Commodore C64 key combinations to select the characters.

Inspired by the [PETSCII Reference](https://style64.org/petscii/) application from <https://style64.org/>.

## Initial Exploration

The [style64-org-petscii](#style64-org-petscii) directory contains a modified version of the [PETSCII Reference](https://style64.org/petscii/) app. The introduced changes include:

1. When clicking on a character, also highlight all characters that are selected by including the same physical base key
   - For example, when selecting the character _A_, also highlight the characters with the key combinations _Shift-A_, _CBM-A_, and _Control->_
   - Conversely, when selecting, for example, the character with the key combination _Shift-A_, also highlight the characters with key combinations _CBM-A_, _Control-A_, and just _A_
2. Add an interactive legend for key combination types (_Shift-*_, _CBM-*_, _Control-*_ key combinations and just the bare key itself)
  - For example, when clicking on the _Shift-*_ legend item, highlight all characters that have a key combination that includes the _Shift_ key
  - Also display the count of characters in each key combination group when clicking on a legend item

The changes have been implemented by vibe coding with Gemini CLI.
