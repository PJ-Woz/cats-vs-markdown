How Markdown is Processed by Wordfast Pro 7 and Trados Studio 2022 <!-- omit in toc -->
===

<!-- This here is a comment. And I'd like to create a TOC below -->
<!-- Use this: https://www.markdownguide.org/cheat-sheet/ -->
<!-- Things I need to insert:
- HTML tags, like <code></code>
- (funny thing that markdown kinda works here)
-  -->

- [Introduction](#introduction)
  - [What is a CAT?](#what-is-a-cat)
  - [Why is This Important?](#why-is-this-important)
- [Markdown Syntax](#markdown-syntax)
  - [General Information](#general-information)
  - [Basic Syntax](#basic-syntax)
    - [Header](#header)
    - [Bold](#bold)
    - [Italic](#italic)
    - [Strikethrough](#strikethrough)
    - [Ordered List](#ordered-list)
    - [Unordered List](#unordered-list)
    - [Combination of Basic Syntax](#combination-of-basic-syntax)
  - [Links](#links)
    - [Links to Sections with Headers](#links-to-sections-with-headers)
    - [Links to Files](#links-to-files)
    - [Links to Images](#links-to-images)
    - [Links to Websites](#links-to-websites)
    - [Links to YouTube](#links-to-youtube)
    - [Syntax for Links](#syntax-for-links)
  - [Quotations](#quotations)
    - [Blockquote](#blockquote)
    - [Inline Code](#inline-code)
    - [Block Code](#block-code)
  - [Extended Syntax](#extended-syntax)
    - [Tables](#tables)
    - [Task List](#task-list)
    - [Emoji](#emoji)
    - [Highlight](#highlight)
    - [Subscript](#subscript)
    - [Superscript](#superscript)
    - [Footnotes](#footnotes)
    - [Ignoring Markdown Formatting](#ignoring-markdown-formatting)
    - [Comments to Be Omitted](#comments-to-be-omitted)
  - [Summary](#summary)
- [HTML and Other Tags](#html-and-other-tags)
  - [General Information](#general-information-1)
  - [Paragraph](#paragraph)
  - [Code](#code)
  - [Collapsed Section](#collapsed-section)
  - [Keyboard keys](#keyboard-keys)
  - [Definition](#definition)
  - [Highlight](#highlight-1)
  - [Subscript](#subscript-1)
  - [Superscript](#superscript-1)
  - [Combination of Tags and Markdown Syntax](#combination-of-tags-and-markdown-syntax)
  - [Summary](#summary-1)
- [Conclusion](#conclusion)
- [Sources](#sources)

# Introduction

<p>I wrote this file to test how two Computer-Aided Translation programs – Wordfast Pro 7 and Trados 2022 – read Markdown files.</p>

## What is a CAT?
[Computer-Aided Translation](https://en.wikipedia.org/wiki/Computer-assisted_translation) software (usually known as CAT) is a program that helps translators translate various files, including Markdown *.md files.

There are **many** diferent CATs. Two of them are *Wordfast Pro* and *Trados Studio 2022*.
## Why is This Important?
Markdown files have unusual formatting. The syntax for __bold__ can be for example: `__bold__`.  
The question arises: Will a CAT know which symbol is part of Markdown syntax and which is used as part of the text?

And to make it even spicier, I also included a few HTML tags to see how they are read in combination with Markdown syntax.

We'll learn soon enough.

# Markdown Syntax

## General Information

I'll check the following Markdown syntax:
1. [Basic syntax](#basic-syntax):
   1. [Header](#header)
   2. [Bold](#bold)
   3. [Italic](#italic)
   4. [Strikethrough](#strikethrough)
   5. [Ordered list](#ordered-list)
   6. [Unordered list](#unordered-list)
2. [Links](#links):
   1. [Links to sections with headers](#links-to-sections-with-headers)
   2. [Links to files](#links-to-files)
   3. [Links to images](#links-to-images)
   4. [Links to websites](#links-to-websites)
   5. [Links to YouTube](#links-to-youtube)
3. [Quotations](#quotations):
   1. [Block quote](#blockquote)
   2. [Inline code](#inline-code)
   3. [Block code](#block-code)
4. [Extended syntax](#extended-syntax):
   1. [Tables](#tables)
   2. [Definition](#definition)
   3. [Task list](#task-list)
   4. [Emoji](#emoji)
   5. [Highlight](#highlight)
   6. [Subscript](#subscript)
   7. [Superscript](#superscript)
   8. [Footnotes](#footnotes)
   9. [Ignoring Markdown formatting](#ignoring-markdown-formatting)
   10. [Comments to be omitted](#comments-to-be-omitted)

---

This will allow us to see which elements of Markdown syntax are – or **are not** – read by two CATs:
- _Wordfast Pro_
- _Trados Studio 2022_

## Basic Syntax
This section contains basic Markdown syntax.

### Header

I've used three types of headers in this text.

Syntax:
```
# Header 1
## Header 2
### Header 3
```

### Bold

**This text is in bold.**  
__This text is in bold.__

Syntax:
- `**This text is in bold.**`
- `__This text is in bold.__`

### Italic

*This text is in italic.*  
_This text is in italic._

Syntax:
- `*This text is in italic.*`
- `_This text is in italic._`

### Strikethrough
~~This text is in strikethrough.~~

Syntax: `~~This text is in strikethrough.~~`

### Ordered List
This is a sample ordered list:
1. Item 1
2. Item 2
3. Item 3
   1. Subitem 3.1
   2. Subitem 3.2

Syntax:
```
1. Item 1
2. Item 2
3. Item 3
   1. Subitem 3.1
   2. Subitem 3.2
```

### Unordered List
This is a sample unordered list:
- Item 1
- Item 2
- Item 3
  - Subitem 3
  - Subitem 3

Syntax:
```
- Item 1
- Item 2
- Item 3
  - Subitem 3
  - Subitem 3
```
### Combination of Basic Syntax

1. *Item with **very important** text*
   - this **simply ~~*wrong*~~**
   - this is __very _important___ as well
2. Another _**combination** of __bold__ and italic_
   1. ~~this is *__bold__ but folly*, so I crossed it out~~

Syntax:
```
1. *Item with **very important** text*
   - this **simply ~~*wrong*~~**
   - this is __very _important___ as well
2. Another _**combination** of __bold__ and italic_
   1. ~~this is *__bold__ but folly*, so I crossed it out~~
```
  
## Links
Here we'll see how different types of links are interpreted by *Wordfast Pro* and *Trados Studio 2022*.

### Links to Sections with Headers
The link to section on [**Bold** is here](#bold).

### Links to Files
The link to [a Markdown file in the __repository__ is _here_](Project-Woźnikowski-2022-11-27.md).

### Links to Images
1. The link to [an image in the **repository** is *here*](images/IMG_20200401_210429.jpg).
2. The link to a displayed image in the repository is here:
   
   ![Shark](images/IMG_20200401_210429.jpg)
3. The link to a displayed image in the repository with a hover text is here:
   
   ![Shark](images/IMG_20200401_210429.jpg "A Technical Writer Shark")
4. The link to a displayed image from the internet:
   
   ![Cieszyn](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e2/2012_Powiat_cieszy%C5%84ski%2C_Cieszyn%2C_Rynek%2C_Fontanna_%C5%9Bw._Floriana_02.jpg/310px-2012_Powiat_cieszy%C5%84ski%2C_Cieszyn%2C_Rynek%2C_Fontanna_%C5%9Bw._Floriana_02.jpg "Cieszyn")

### Links to Websites
The link to [my website Translatorion.com is here](https://translatorion.com/).

### Links to YouTube
The link to an embedded David Bowie video on YouTube is here:

[![I am a DJ](http://img.youtube.com/vi/MRRmU_pOXnk/0.jpg)](http://www.youtube.com/watch?v=MRRmU_pOXnk "I am what I play").

### Syntax for Links

Syntax example: `![Shark](images/IMG_20200401_210429.jpg "A Technical Writer Shark")`

## Quotations

This section contains various ways of quoting text or code.

### Block Quote

> This is an example of a quote.
> 
> This quote ~~doesn't~~ also includes __basic syntax__ and a [*link*](https://en.wikipedia.org/wiki/Link,_West_Virginia).


Syntax:
```
> This is an example of a quote.
> 
> This quote ~~doesn't~~ also includes __basic syntax__ and a [*link*](https://en.wikipedia.org/wiki/Link,_West_Virginia).
```

### Inline Code

This is an example of a sentence with an inline code of a text in `**bold** and _italic_`.

Syntax:
```
`**bold** and _italic_`
```

### Block Code

This is an example of block code with:
```
1. __Bold__
2. *Italic*
   1. ~~Strikethrough~~
3. > Quotation:
   > - unordered list
4. Link [to a very wise person](https://en.wikipedia.org/wiki/Arthur_Schopenhauer)
```

Syntax: ` ```code``` `

## Extended Syntax

This section contains extended syntax.

### Tables

| No. | Name | Surname | Photo | Age |
| :--- | :---: | :---: | --- | ---: |
| 1. | [**John _the Fearless_**](https://en.wikipedia.org/wiki/John_the_Fearless) | [__Valois__](https://en.wikipedia.org/wiki/House_of_Valois) | ![John the Fearless](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Flemish_School_-_Lille_-_John%2C_Duke_of_Burgundy.jpg/173px-Flemish_School_-_Lille_-_John%2C_Duke_of_Burgundy.jpg "John the Fearless")|   48 |
| 2. | [**Philip *the Good***](https://en.wikipedia.org/wiki/Philip_the_Good) | [**Valois**](https://en.wikipedia.org/wiki/House_of_Valois) | ![Philip the Good](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a4/Philip_the_good.jpg/170px-Philip_the_good.jpg "Philip the Good") | 70 |
| 3. | [__Charles *the Bold*__](https://en.wikipedia.org/wiki/Charles_the_Bold) | [__Valois__](https://en.wikipedia.org/wiki/House_of_Valois) | ![Charles the Bold](https://upload.wikimedia.org/wikipedia/commons/thumb/0/03/Charles_the_Bold_1460.jpg/154px-Charles_the_Bold_1460.jpg "Charles the Bold") | 44 |
| 4. | [__Mary *of Burgundy*__](https://en.wikipedia.org/wiki/Mary_of_Burgundy) | [~~Valois~~](https://en.wikipedia.org/wiki/House_of_Valois) [**Habsburg**](https://en.wikipedia.org/wiki/House_of_Habsburg) | ![Mary of Burgundy](https://upload.wikimedia.org/wikipedia/commons/thumb/8/88/Mary_of_Burgundy_%281458%E2%80%931482%29%2C_by_Netherlandish_or_South_German_School_of_the_late_15th_Century.jpg/169px-Mary_of_Burgundy_%281458%E2%80%931482%29%2C_by_Netherlandish_or_South_German_School_of_the_late_15th_Century.jpg "Mary of Burgundy") | 25 |

Syntax (part):
```
| No. | Name | Surname | Photo | Age |
| :--- | :---: | :---: | --- | ---: |
| 1. | [**John _the Fearless_**](https://en.wikipedia.org/wiki/John_the_Fearless) | [__Valois__](https://en.wikipedia.org/wiki/House_of_Valois) | ![John the Fearless](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Flemish_School_-_Lille_-_John%2C_Duke_of_Burgundy.jpg/173px-Flemish_School_-_Lille_-_John%2C_Duke_of_Burgundy.jpg "John the Fearless")|   48 |
```

### Task List

This is a sample task list:
- [ ] Task **one**
- [ ] Task *two*
- [ ] _**Task** three_
  - [ ] ___Subtask three.one___
  - [ ] ~~Subtask three.two~~
- [ ] *__Task four__*

Syntax: `- [ ] task name`

### Emoji

This is a sample list of emojis:
- :wink:
- :uk:
- :cat:
- :tm:
- :aquarius:

Syntax: `:wink:`

### Highlight

This is a sample Markdown ==highlight==. ==Not all== Markdown processors interpret this highlighting.

Syntax: `==text==`.

### Subscript

This is a sample Markdown ~subscript~. ~Not all~ Markdown processors interpret this subscript.

Syntax: `~text~`.

### Superscript

This is a sample Markdown ^superscript^. ^Not all^ Markdown processors interpret this superscript.

Syntax: `^text^`.

### Footnotes

This is a sentence with a footnote.[^1]

Syntax: `This is a sentence with a footnote.[^1]`

This is another footnote. [^bignote]

Syntax: `This is another footnote. [^bignote]`

[^1]: Additional information

[^bignote]: Additional information

### Ignoring Markdown Formatting

A short list of ignored Markdown formatting:
- \*\*bold**
- \_italic_
- \~~strikethrough~~
- \`\*code\*`

Syntax: \\\*\\\*bold**

### Comments to Be Omitted

Below this sentence there's a comment to be omitted by Markdown processors:

<!--- Comment --->

Syntax: `<!--- Comment --->`

## Summary

**This _sums_ ~~~down~~~ ^up^:**
- ___the `Basic` [Markdown](https://en.wikipedia.org/wiki/Markdown) Syntax :sweat_smile:___

# HTML and Other Tags

## General Information

I'll check the following HTML and other tags:
1. [Paragraph](#paragraph)
2. [Code](#code)
3. [Collapsed Section](#collapsed-section)
4. [Keyboard keys](#keyboard-keys)
5. [Definition](#definition)
6. [Highlight](#highlight-1)
7. [Subscript](#subscript-1)
8. [Superscript](#superscript-1)
9. [Combination of tags and Markdown syntax](#combination-of-tags-and-markdown-syntax)

## Paragraph

<p>This is lorem ipsum: lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur ullamcorper ante sit amet aliquet convallis. Integer mollis urna quis velit mattis facilisis.</p>
<p>Vestibulum pulvinar sed eros vitae eleifend. Mauris et ligula metus. Nunc elementum vestibulum arcu quis ultricies. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.</p>

Syntax: `<p>Lorem ipsum</p>`

## Code

This is a sample code:
<code>\*\*bold** \_italic_</code>

Syntax: `<code>\*\*bold** \_italic_</code>`

## Collapsed Section

This is a normal section.

<details><summary>Unroll another section</summary>
<p>

*Text* with __different__ ~~formatting~~.

| No. | Name | Surname |
| --- | --- | --- |
| 1. | Agnes | **Aardvark** |
| 2. | Burt | _Butterly_ |

A very [important link](https://youtu.be/dQw4w9WgXcQ?t=43).

</p>
</details>

Syntax (part):
```
<details><summary>Unroll another section</summary>
<p>

*Text* with __different__ ~~formatting~~.

</p>
</details>
```

## Keyboard keys

Use <kbd>W</kbd>, <kbd>S</kbd>, <kbd>A</kbd>, <kbd>D</kbd> keys to move your character in a video game.

And never touch the <kbd>Windows</kbd> key!

Syntax: `<kbd>Windows</kbd>`

## Definition

This is a sample definition.
<dl>
"Definition":
<dt> a statement that explains the meaning of a word or phrase </dt>
<dt> a description of the features and limits of something </dt>
</dl>

From [Cambridge Dictionary](https://dictionary.cambridge.org/pl/dictionary/english/definition).

Syntax:
```
<dl>
"Definition":
<dt> a statement that explains the meaning of a word or phrase </dt>
<dt> a description of the features and limits of something </dt>
</dl>
```

## Highlight

This is a sample HTML <mark>highlight</mark>. <mark>Not all</mark> Markdown processors interpret this highlighting.

Syntax: `<mark>text</mark>`

## Subscript

This is a sample HTML <sub>subscript</sub>. <sub>Not all</sub> Markdown processors interpret this subscript.

Syntax: `<sub>text</sub>`

## Superscript

This is a sample HTML <sup>superscript</sup>. <sup>Not all</sup> Markdown processors interpret this superscript.

Syntax: `<sup>text</sup>`

##  Combination of Tags and Markdown Syntax

*This* is __a combination__ of <mark>various</mark> <kbd>key</kbd> <sup>components</sup> of [Markdown](https://en.wikipedia.org/wiki/Markdown) and <code>tags</code>.

Syntax:
```
*This* is __a combination__ of <mark>various</mark> <kbd>key</kbd> <sup>components</sup> of [Markdown](https://en.wikipedia.org/wiki/Markdown) and <code>tags</code>.
```

## Summary

I'm aware that placing Markdown syntax inside HTML tags, like `<p>paragraph</p>`, turns them off in some processors.

# Conclusion

I hope this extensive — but definitely not exhaustive — list of Markdown and HTML tags will be a good test for *Wordfast Pro* and *Trados Studio 2022*.

I've written this Markdown file in Visual Studio Code that doesn't show all Markdown syntax in the preview window, i.e.:
 - highlight
 - subscript
 - superscript
 - footnotes

Also, not all Markdown syntax or HTML tags work in Github viewer.

# Sources

1. [Markdownguide.org](https://www.markdownguide.org/)
2. [Keyboard glyphs](https://meta.stackexchange.com/questions/5527/keyboard-glyphs)
3. [Collapsed sections](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-collapsed-sections)