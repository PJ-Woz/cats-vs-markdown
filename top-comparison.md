---
title: Comparison of CATs
layout: default
nav_order: 7
---
Comparison of CATs
===

## Overview

This section shows a comparison of Phrase, Trados Studio 2022, and Wordfast Pro 8.

Table 1 covers every feature presented in the test file and every CAT.

Table 2 shows the summary results from Table 1.

The usability index of a CAT is measured by the sum of the number of `✔️YES` and of the number of `⚠️️DEPENDS`.

However, the usability index is only a simple measure. The results are additionally discussed because some features are more important or make translation a more fail-proof process.

### Symbols and their meanings

There are three symbols used in the table:
- `✔️YES` means that a given feature works in all tested settings
- `⚠️️DEPENDS` means that a given feature works in some settings. It also means that it may cause problems when importing the file or show issues in the output file
- `❌NO` means that a given feature does not work in any setting


## Comparison

 | No. | Feature                                    | Phrase    | Trados    | Wordfast  |
| :--- | :--------------------------------------- | :---------: | :---------: | :---------: |
| 1   | Basic syntax                            | ⚠️️DEPENDS | ✔️YES     | ⚠️️DEPENDS |
| 2   | Header                                  | ✔️YES     | ✔️YES     | ✔️YES     |
| 3   | Bold                                    | ✔️YES     | ✔️YES     | ✔️YES     |
| 4   | Italic                                  | ✔️YES     | ✔️YES     | ✔️YES     |
| 5   | Strikethrough                           | ⚠️️DEPENDS | ✔️YES     | ✔️YES     |
| 6   | Ordered list                            | ⚠️️DEPENDS | ✔️YES     | ✔️YES     |
| 7   | Unordered list                          | ⚠️️DEPENDS | ✔️YES     | ✔️YES     |
| 8   | Combination of basic syntax             | ⚠️️DEPENDS | ✔️YES     | ⚠️️DEPENDS |
| 9   | Links                                   | ⚠️️DEPENDS | ⚠️️DEPENDS | ⚠️️DEPENDS |
| 10  | Links to sections with headers          | ❌NO       | ❌NO       | ⚠️️DEPENDS |
| 11  | Links to files                          | ✔️YES     | ✔️YES     | ✔️YES     |
| 12  | Links to images                         | ✔️YES     | ✔️YES     | ✔️YES     |
| 13  | Links to websites                       | ✔️YES     | ✔️YES     | ✔️YES     |
| 14  | Links to YouTube                        | ✔️YES     | ✔️YES     | ✔️YES     |
| 15  | Links with hover text                   | ✔️YES     | ⚠️️DEPENDS | ⚠️️DEPENDS |
| 16  | Quotations                              | ⚠️️DEPENDS | ⚠️️DEPENDS | ⚠️️DEPENDS |
| 17  | Blockquote                              | ✔️YES     | ✔️YES     | ✔️YES     |
| 18  | Inline code                             | ⚠️️DEPENDS | ❌NO       | ❌NO       |
| 19  | Code block                              | ⚠️️DEPENDS | ⚠️️DEPENDS | ❌NO       |
| 20  | Extended syntax                         | ⚠️️DEPENDS | ⚠️️DEPENDS | ⚠️️DEPENDS |
| 21  | Tables                                  | ⚠️️DEPENDS | ✔️YES     | ⚠️️DEPENDS |
| 22  | Task list                               | ✔️YES     | ✔️YES     | ✔️YES     |
| 23  | Emoji                                   | ⚠️️DEPENDS | ✔️YES     | ✔️YES     |
| 24  | Highlight                               | ⚠️️DEPENDS | ⚠️️DEPENDS | ⚠️️DEPENDS |
| 25  | Subscript                               | ⚠️️DEPENDS | ⚠️️DEPENDS | ⚠️️DEPENDS |
| 26  | Superscript                             | ⚠️️DEPENDS | ⚠️️DEPENDS | ⚠️️DEPENDS |
| 27  | Footnotes                               | ⚠️️DEPENDS | ❌NO       | ✔️YES     |
| 28  | Ignoring Markdown formatting            | ✔️YES     | ✔️YES     | ✔️YES     |
| 29  | Comments to be omitted                 | ❌NO       | ⚠️️DEPENDS | ❌NO       |
| 30  | HTML and other tags                     | ⚠️️DEPENDS | ⚠️️DEPENDS | ⚠️️DEPENDS |
| 31  | Paragraph                               | ✔️YES     | ✔️YES     | ✔️YES     |
| 32  | Code                                    | ✔️YES     | ✔️YES     | ✔️YES     |
| 33  | Collapsed section                       | ✔️YES     | ⚠️️DEPENDS | ⚠️️DEPENDS |
| 34  | Keyboard keys                           | ✔️YES     | ✔️YES     | ✔️YES     |
| 35  | Definition                              | ✔️YES     | ⚠️️DEPENDS | ✔️YES     |
| 36  | Highlight                               | ✔️YES     | ✔️YES     | ✔️YES     |
| 37  | Subscript                               | ✔️YES     | ✔️YES     | ✔️YES     |
| 38  | Superscript                             | ✔️YES     | ✔️YES     | ✔️YES     |
| 39  | Combination of tags and Markdown syntax | ✔️YES     | ✔️YES     | ✔️YES     |
| 40  | Pure HTML syntax with JavaScript        | ✔️YES     | ⚠️️DEPENDS | ✔️YES     |

*Table 1: Comparison of features and the CATs*

## Usability index

The table below shows the summary results for `✔️YES`, `⚠️️DEPENDS`, and `❌NO`.

| Total     | Phrase | Trados | Wordfast |
| :--------- | :------: | :------: | :--------: |
| ✔YES     | 21     | 24     | 24       |
| ❌NO       | 2      | 3      | 3        |
| ⚠️DEPENDS | 17     | 13     | 13       |
| ✔YES + ⚠️DEPENDS | **38**     | 37     | 37       |

*Table 2: Summary of the results*

As can be seen, Trados and Wordfast are tied for the first place on `✔️YES`.

Phrase is on the first place on `⚠️️DEPENDS`.

Based on the data, Phrase is the most usable CAT out of the three. However, only by a small margin. Trados and Wordfast are tied for second.

## Discussion of the results

### [Phrase](phrase-00-overview)

Even though Phrase scored first, there are some reservations.

On the downside, Phrase requires adequate settings for even the basic syntax to work as intended. Moreover, it can create issues in the output file. When it comes to features, it does not support comments to be omitted and Markdown reference. Especially Markdown reference can be a serious issue for knowledge bases created in Markdown.

On the upside, Phrase has some advantages over Trados and Wordfast. It has settings that can be configured by the user to adequately capture what elements need additional filtering. Also, it is the only CAT that supports translation of inline code and code blocks. These settings can be also turned off, so if code does not have to be translated, it is not visible in the editor. This protects against accidental edits.

**Verdict**: Good solution, covers almost everything, a lot can be configured by the user. However, the need for proper configuration is a disadvantage for less knowledgeable translators.

### [Trados Studio 2022](trados-00-overview)

As an industry standard software, Trados is a solid solution for translating Markdown files.

Even though it does not have as many settings as Phrase or even Wordfast, it works well with many features on basic filters. However, some settings create errors, which may cause confusion and delay[.](resources/images/confusion-and-delay.jpg)

The major disadvantage of Trados is the inability to translate inline code and Markdown reference. Just like Phrase, lack of Markdown reference can be a serious issue for knowledge bases created in Markdown. No support for footnotes only reinforces this drawback. Also, unpredictable behaviour of hover text is an issue. Finally, if HTML is filtered with the `Embedded Content Plain Text v 1.0.0.0` setting, it is shown as text, with all the code. This increases the risk of accidental edits.

On the upside, Trados is the only CAT in which comments can be translated and this may be useful in certain situations. Also, once configured, it works well with vast majority of tested features.

**Verdict**: Good solution, an all-rounder that does not require much configuration. However, some configurations do not work, cause errors, or are not fail-proof, which may be problematic for translators.

### [Wordfast Pro 8](wordfast-00-overview)

As a [second-to-Trados](https://go.proz.com/blog/cat-tool-use-by-translators-what-are-they-using), Wordfast is also a solid solution for translating Markdown files. However, the overall impressions are mixed.

On the downside, Wordfast behaves bizarrely. It generated an error caused by a combination of different formatting tags. Tables work poorly in some settings. Also, even though it provides a lot of settings, it is only an illusion of choice. The majority of them would be always ticked as there are not many cases in which it would be advisable not to import table headers, image title, or alt text. The biggest drawback of Wordfast is that comments, inline code, and code blocks cannot be translated.

On the upside, the formatting error was caused by a fringe case that most likely will not occur in standard writing. Moreover, it can be reformulated to work. Also, Wordfast is the only CAT that supports translation of Markdown references, which makes it a perfect tool for e.g. knowledge bases because it also supports footnotes. Lastly, Wordfast reads embedded HTML without any issues, whether it is embedded fully between `<html></html>` tags or any other tags like `<sub></sub>`.

**Verdict**: Good solution and it would be the best if it supported translation of inline code or code blocks. Possibility of translating Markdown reference is a game changer in comparison with the other CATs. However, it has a disappointing illusion of the choice of settings, as many of them should be default.

### Which CAT to choose?

All three CATs come close and there is no single best solution. All three are ahead of the others in some respects, while stunningly fail with regard to other features. Much depends on what needs to be translated.

- Phrase is a good solution for documentation with simple structure without references. It is also good for situations that require user-defined settings. It is definitely the best when it comes to code with translatable content.

- Trados is also a good solution and is very similar to Phrase. However, it offers less configuration, choosing appropriate settings is crucial, and it does not support inline code and references.

- Wordfast is best for texts that have a lot of references and which do not require code to be translated. Once all settings are checked, it can tackle most cases.

If the Markdown file contains very complex features and many elements like comments, inline code, code block, or Markdown references, a good solution would be to use several CATs. However, in some cases it may not be viable. As CATs which are most universal, Phrase and Wordfast would cover almost all crucial features. Generally, much depends on the files to be translated and features they include. A good idea may be to compare which CATs work best with a given use case: if the files have a lot of tables, code to be translated, links to be edited, etc. In the most extreme case like the text file, however, all three CATs would be needed to translate such file completely.

On a general level, successful translation of Markdown projects in CATs requires special considerations, which are covered in the next section.

---

Go to section: [*General recommendations*](top-general-rec)