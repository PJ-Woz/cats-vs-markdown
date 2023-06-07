---
title: What is a CAT?
layout: default
nav_order: 2
parent: Overview
---
# What is a CAT?

A **Computer-Aided Translation** software (in short: a **CAT**) is a program that helps translators translate. Translation is still done by a human, but the CAT facilitates this process with inbuilt features.

The primary feature of a CAT is a text editor. A CAT can open many different source formats, like `.docx`, `HTML`, and Markdown `.md` files. A file to be translated is imported into the CAT and divided into **segments**. A segment is usually a sentence, but it may be also, e.g., an item from a list or a header. A segment has its counterpart in the target language that is filled in with translation by the translator.

In segments, the majority of formatting is not displayed, e.g., colour formatting or a website address. Some CATs display bold or italics, but this is not always the case. However, the CAT does not remove such formatting features permanently from the file, as they are required in the translated file. Such formatting is displayed as non-editable **tags**. They are non-editable, because they may also include text that is not to be translated, like a website address.

Another important feature of the CAT is translation memory. A translation memory is a database that stores segments with their translated counterparts. The translated segments may be retrieved in the future if there is another segment that is exactly the same (a 100% match) or if it is similar (a fuzzy match).

CATs offer many other tools and functionalities, but these are not relevant to this project, so they are not discussed.

# What CATs are there?

There are [many different CAT programs](https://www.g2.com/categories/computer-assisted-translation "various CAT programs"). Some are open-source, some are cloud-based, while some are completely desktop-based.

In this project, three CATs are analysed to test how they import and export Markdown files:
- [Phrase](#phrase)
- [Trados Studio 2022](#trados-studio-2022)
- [Wordfast Pro 8](#wordfast-pro-8)

### Phrase

[Phrase](https://phrase.com/) (earlier: Memsource) is a cloud-based translation management system, which also includes a CAT tool. It is completely web-based, meaning it is used via a web browser.

In this project, Phrase CAT web editor ver. 23.18.1 was used.

[*Skip to section on Markdown in Phrase*.](phrase-01-settings)

### Trados Studio 2022

[Trados Studio](https://www.trados.com/products/trados-studio/whats-new-studio-2022.html) is the oldest CAT software and often regarded as an industry standard. It works as a desktop application.

In this project, Trados Studio 2022 ver. 17.0.4.13209 was used.

[*Skip to section on Markdown in Trados Studio 2022*](trados-01-settings)

### Wordfast Pro 8

[Wordfast](https://www.wordfast.com/products/wordfast_pro) is a CAT that started first as an add-on to Microsoft Word (now called Wordfast Classic). Later, it was developed into a desktop application, called Wordfast Pro.

In this project, Wordfast Pro 8 ver. 8.1.0 was used.

[*Skip to section on Markdown in Wordfast Pro 8*](wordfast-01-settings)

---

These CATs import Markdown files. However, they do it differently depending on particular settings.

---

Next section: [*Why is Markdown difficult in translation?*](ref-why-md-difficult)

Skip to section:
- [*Comparison of the three CATs*](top-comparison)
- [*General recommendations for translating Markdown*](top-general-rec)

---

References:
[G2: listings of CAT software](https://www.g2.com/categories/computer-assisted-translation)