---
title: Phrase — summary and recommendations
layout: default
nav_order: 3
parent: Phrase — overview
---
Phrase
===

## Summary

In general, Phrase is a good tool to translate Markdown files when specific settings are applied.

### Advantages

- Rich settings
	- Can be configured with regex and other rules
- Inline code can be translated
- Code block can be translated
- Imports the content of embedded HTML code

### Disadvantages

- Only GitHub flavoured Markdown yields satisfactory results
	- [Plain](phrase-02-results#plain){:target="_blank"} Markdown flavour creates an output file that is useless, as restoring it to a usable state would take much time
- Markdown reference in links cannot be translated, which makes it impossible to translate a table of contents or all other references to headers in Markdown files
- Many different features stop working in the output file, even though they look good in the editor
	- Notable exception: [GitHub flavoured Markdown](phrase-02-results#github-flavoured-markdown){:target="_blank"}
- Comments `<!-- comment example -->` are ignored and cannot be translated
- Emoji is shown as text, which makes it difficult for Machine Translation

## Recommendations for translation of Markdown files in Phrase

This section contains recommendations for technical writers (or generally, authors writing in Markdown) and translators.

### Recommendations for technical writers

- Inform the translator about basic Markdown syntax because some tags can be shown as text
- Inform the translator about HTML or quoted code syntax because the content in the code block is shown as text
- Instruct the translator to use [PHP/Python Markdown Extra](phrase-02-results#php-&#47;-python-markdown-extra){:target="_blank"} or [GitHub Flavoured Markdown](phrase-02-results#github-flavoured-markdown){:target="_blank"} and inform about their limitations
- Instruct the translator **NOT TO USE** [Plain Markdown flavour](phrase-02-results#plain){:target="_blank"}
- If references are to be translated, inform the translator:
	- The references need to be translated in the Markdown file
	- How to open a Markdown file
	- The syntax: one hash symbol, no space between the hash symbol and the first word, small letters, and minus symbol instead of spaces; e.g., the reference to this section should be `#recommendations-for-technical writers`
- If `<!-- comment example -->` comments are to be translated, instruct the translator about:
	- How to open the Markdown file
	- The syntax
	- What is to be translated and what must not be edited
	- Alternatively, break the syntax, so the comment is imported into the CAT, and fix it yourself in the output file
- Inform the translator that the output file may look different from the source file
- Encourage the translator to contact you if the CAT editor shows any characters that are not used in a standard way in the source language as these are most likely tags

### Recommendations for translators

- Use [PHP/Python Markdown Extra](phrase-02-results#php-&#47;-python-markdown-extra){:target="_blank"} if no lists are used, but footnotes are
- Use [GitHub Flavoured Markdown](phrase-02-results#github-flavoured-markdown){:target="_blank"} if lists are used, but not footnotes
- **DO NOT USE** [Plain Markdown flavour](phrase-02-results#plain){:target="_blank"} unless the source file consists of bold and italics only
	- for safety, do not use it at all
- Adapt the settings to your needs — if the inline code or code block do not contain translatable content, uncheck `Include code blocks` and `Exclude code elements` to avoid accidental editing
- Make sure you do not edit something that may be a tag when you translate the content of the inline code or code block
- Contact the technical writer if the source text in the CAT editor shows unexpected characters, as they may be part of Markdown or HTML syntax shown as text
- Make sure you do not edit something that may be a Markdown tag
- Make sure you do not edit an emoji, e.g., `:exploding_head:`
- Carefully check the output file for any missing elements

---

Go to sections:
- [*Trados — overview*](trados-00-overview)
- [*Wordfast Pro 8 — overview*](wordfast-00-overview)
- [*Comparison of CATs*](top-comparison)
- [*General recommendations for translating Markdown*](top-general-rec)