# Spanish language module for RHVoice

This language module contains needed binaries to build and run Spanish voices.

It works in both Castilian and neutral Latin bariants. In the future, we will follow variants with specific rules, like Argentinian Spanish, if someone give us voices of these specific variants, in which have changes of sounds in some phonemes.
If so, these variants will be available by branches of this repository.

## Features

- [Extra] currency support (binaries only, not registered in the core at all): These binaries translates a given currency format to human-speaker readable string. It probably can be available in the future by special c++ code for it.
  - Example: $1.25 (1 dólar y 25 centavos)
- [Extra] date support: it applies the same function than currency, but it is now available for the core and voices. This takes a specific format, `dd/mm/yyyy` in the text.
  - Example: 23/07/2025 (the voice will say veintitrés de julio del dos mil veinticinco)
- Pronunciation dictionary: this is a set of the most comon foreign entries, that which needs to be pronounced as such.
  - Browsers: Chrome (croum) Firefox (fáirfox)
  - Places: Texas (tejas)
- Pitch marks for exclaim and question sentences. All voices will interpret them by raising or lowering pitch, according to the pitch range of the speaker.
- [Extra] Fanci normalization: we know that NVDA has own unicode normalization support. However, RHVoice is multiplatform, and these are fully supported in this language module, useful to read poems with stylized text.
- [Extra] SAPM (Sentence-Aware Prosody Modelling): It correctly interprets prosody of Spanish words that have more than one context, and a context handles a different accentuation or stress. Rich prosody ensured, and improves experience for screen reader users.
- [Extra] Special skills to handle initialisms (AKA **siglas** in Spanish): This integrates special rules, especially in tokenization, to interpret initialisms as letter sequences in an efficient way.
  - Examples: NVDA, CNE, ADN.
