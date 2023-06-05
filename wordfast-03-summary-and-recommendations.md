# Summary

In general, Wordfast Pro 8 is a good tool to translate Markdown files despite the import error in the beginning.

## Advantages

- Markdown reference in links can be translated, which makes it possible to translate a table of contents and all other references to headers in Markdown files
- Many filter settings allow rich configuration options for importing Markdown files
- Imports the content of embedded HTML code

## Disadvantages

- Inline code is ignored and cannot be translated
- Code block is ignored and cannot be translated
- Comments `<!-- comment example -->` are ignored and cannot be translated
- Bizarre behaviour of tables
- Very complex combinations of Markdown tags or with HTML tags may cause problems or make the Markdown tags shown as text; however, in the case of HTML tags this has more to do with the general behaviour between HTML and Markdown tags

# Recommendations for translation of Markdown files in Wordfast Pro

This section contains recommendations for technical writers (or generally, authors writing in Markdown) and translators.

## Recommendations for technical writers

- Avoid combining bold, italic, and strikethrough — some combinations may cause importing errors
- Inform the translator about basic Markdown syntax, because some tags can be shown as text
	- If references are translated, instruct the translator how to translate references and what the syntax is: one hash symbol, no space between the hash symbol and the first word, small letters, and minus symbol instead of spaces; e.g. the reference to this section should be `#recommendations-for-technical writers`
- If inline code, code block, or `<!-- comment example -->` comments are to be translated, instruct the translator about:
	- How to open the Markdown file
	- The syntax
	- What is to be translated and what must not be edited
	- Alternatively, break the syntax, so the comment is imported into the CAT, and fix it yourself in the output file
- If extended Markdown syntax or HTML tags, inform the translator that there may be characters that are not used in a standard way in the source language and tell the translator what to do with them
- Encourage the translator to contact you if the CAT editor shows any characters that are not used in a standard way in the source language as these are most likely tags

## Recommendations for translators

- Tick all settings for best performance, even if it means pasting links
- Contact the technical writer if the source text in the CAT editor shows unexpected characters, as they may be part of Markdown or HTML syntax shown as text
- Make sure you do not edit something that may be a tag
- Carefully check the output file for any missing elements, especially in tables

---

Go to sections:
- [*Phrase — overview*](phrase-00-overview.md)
- [*Trados Studio 2022 — overview*](trados-00-overview.md)
- [*Comparison of CATs*](top-comparison.md)
- [*General recommendations for translating Markdown*](top-general-rec.md)

---
[Back to top](#summary)