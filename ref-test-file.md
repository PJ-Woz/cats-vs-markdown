---
title: The test file
layout: default
nav_order: 3
---
## The test file

To check the settings of the Markdown filter in Phrase, Trados Studio 2022, and Wordfast Pro 8, a test file was prepared. The assumption was to use all basic and extended Markdown tags in different combinations.

Also, HTML with JavaScript was embedded in the test file, as these are often used in Markdown files. As a result, this use case is also covered in the study.

The test file is a Markdown guidebook. It includes a list of Markdown tags, their syntax, and the expected results are presented. That is why Markdown syntax is omitted in this page.

Go to [the test file](resources/Markdown-in-CAT-test){:target="_blank"}.

## Definitions

In the study, special phrases are used with the following meanings:
1. <kbd>&#128008;CAT EDITOR ISSUE</kbd>  — this means that there is a problem in the CAT editor
2. `CAT tag` — this means a non-editable placeholder that replaces a syntax element from the input file in the CAT editor
3. `ignored` — this means that a given item is not displayed in the CAT editor
4. <kbd>&#128228;OUPUT FILE ISSUE</kbd> — this means that there is a problem with the file exported from the CAT even though there were no issues in the CAT editor
5. <kbd>&#128680;REALLY!</kbd> — this means a surprising result
6. `reference` — this means the part of a Markdown link that is in parentheses, e.g. in `[Shark](IMG_20200401_210429.jpg)`, it is `IMG_20200401_210429.jpg`. It can be an [**URL**](#URL), a path to a file, or a header anchor
7. `shown as text` — this means that Markdown or HTML tags are displayed with normal characters instead of CAT tags inserted in the editor
	IMPORTANT: This means that such tags can be accidentally edited, which will result in a faulty output file

---

Next section: [*Phrase — overview*](phrase-00-overview)

Skip to section:
- [*Trados Studio 2022 — overview*](trados-00-overview)
- [*Wordfast Pro 8 — overview*](wordfast-00-overview)
- [*Comparison of CATs*](top-comparison)
- [*General recommendations for translating Markdown*](top-general-rec)