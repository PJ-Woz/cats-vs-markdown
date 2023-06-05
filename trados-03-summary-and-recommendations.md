---
title: Trados Studio 2022 — summary and recommendations
layout: default
nav_order: 3
parent: Trados Studio 2022  — overview
---
# Summary

In general, Trados Studio 2022 is a good tool to translate Markdown files. However, it shows strange behaviour and errors in some of the settings.

## Advantages

- Imports a lot of content in default settings, e.g.:
	- link descriptions
	- hover text
- Code block can be translated. This is useful when you need to translate comments in code or messages from developers
- Comments `<!-- comment example -->` can be translated
- Imports the content of embedded HTML code, but only in `Html Embedded Content 5 2.0.0.0`

## Disadvantages

- Bizarre behaviour of hover text between different references
- Markdown reference in links cannot be translated, which makes it impossible to translate a table of contents or all other references to headers in Markdown files
- Inline code is ignored and cannot be translated
- HTML in the `Embedded Content Plain Text v 1.0.0.0` filter is shown as text, which increases the risk of accidental editing

# Recommendations for translation of Markdown files in Trados Studio

This section contains recommendations for technical writers (or generally, authors writing in Markdown) and translators.

## Recommendations for technical writers

- Inform the translator about basic Markdown syntax because tags in code block are shown as text
- If references are to be translated, inform the translator:
	- The references need to be translated in the Markdown file
	- How to open a Markdown file
	- The syntax: one hash symbol, no space between the hash symbol and the first word, small letters, and minus symbol instead of spaces; e.g., the reference to this section should be `#recommendations-for-technical writers`
- Inform the translator about HTML or quoted code syntax, because the content in the code block is shown as text
- If possible, use code block even for inline code because inline code cannot be translated
- Encourage the translator to contact you if the CAT editor shows any characters that are not used in a standard way in the source language as these are most likely tags
- Be aware that some content between different HTML tags may or may not be imported into Trados and, as a result, translated

## Recommendations for translators

- Adapt the settings to your needs — if the embedded HTML does not contain content to be translated, uncheck the `Translate HTML block` box 
	- This way you do not risk accidental editing of the HTML code
- Do not edit something that may be a tag when you translate the content of the code block
- Contact the technical writer if the source text in the CAT editor shows unexpected characters, as they may be part of Markdown or HTML syntax shown as text
- Be aware that some content between different HTML tags may or may not be imported into Trados and, as a result, translated
- Carefully check the output file for any missing elements or elements placed incorrectly, e.g., hover text

---

Go to sections:
- [*Phrase — overview*](phrase-00-overview)
- [*Wordfast Pro 8 — overview*](wordfast-00-overview)
- [*Comparison of CATs*](top-comparison)
- [*General recommendations for translating Markdown*](top-general-rec)

---