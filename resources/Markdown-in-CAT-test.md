How Markdown is Processed by Wordfast Pro 8, Trados Studio 2022, and Phrase<!-- omit in toc -->
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
    - [Links with Hover Text](#links-with-hover-text)
    - [Syntax for Links](#syntax-for-links)
  - [Quotations](#quotations)
    - [Blockquote](#blockquote)
    - [Inline Code](#inline-code)
    - [Code Block](#code-block)
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
  - [Keyboard Keys](#keyboard-keys)
  - [Definition](#definition)
  - [Highlight](#highlight-1)
  - [Subscript](#subscript-1)
  - [Superscript](#superscript-1)
  - [Combination of Tags and Markdown Syntax](#combination-of-tags-and-markdown-syntax)
  - [Pure HTML Syntax with JavaScript](#pure-html-syntax-with-javascript)
  - [Summary](#summary-1)
- [Conclusion](#conclusion)
- [Sources](#sources)

# Introduction

I wrote this file to test how three Computer-Aided Translation programs — Wordfast Pro 8, Trados Studio 2022, and Phrase — read Markdown files.

## What is a CAT?
[Computer-Aided Translation](https://en.wikipedia.org/wiki/Computer-assisted_translation) software (usually known as CAT) is a program that helps translators translate various files, including Markdown *.md files.

There are **many** diferent CATs. Three of them are *Wordfast Pro*, *Trados Studio*, and *Phrase*.
## Why is This Important?
Markdown files have unusual formatting. The syntax for __bold__ can be for example: `__bold__`.  
The question arises: Will a CAT know which symbol is part of Markdown syntax and which is used as part of the text?

And to make it even spicier, I also included a few HTML tags to see how they are read in combination with Markdown syntax.

We'll learn soon enough.

# Markdown Syntax

## General Information

I'll check the following Markdown syntax:
1. [Basic Syntax](#basic-syntax):
   1. [Header](#header)
   2. [Bold](#bold)
   3. [Italic](#italic)
   4. [Strikethrough](#strikethrough)
   5. [Ordered List](#ordered-list)
   6. [Unordered List](#unordered-list)
2. [Links](#links):
   1. [Links to Sections with Headers](#links-to-sections-with-headers)
   2. [Links to Files](#links-to-files)
   3. [Links to Images](#links-to-images)
   4. [Links to Websites](#links-to-websites)
   5. [Links to YouTube](#links-to-youtube)
3. [Quotations](#quotations):
   1. [Blockquote](#blockquote)
   2. [Inline Code](#inline-code)
   3. [Code Block](#code-block)
4. [Extended Syntax](#extended-syntax):
   1. [Tables](#tables)
   2. [Definition](#definition)
   3. [Task List](#task-list)
   4. [Emoji](#emoji)
   5. [Highlight](#highlight)
   6. [Subscript](#subscript)
   7. [Superscript](#superscript)
   8. [Footnotes](#footnotes)
   9. [Ignoring Markdown Formatting](#ignoring-markdown-formatting)
   10. [Comments to Be Omitted](#comments-to-be-omitted)

---

This will allow us to see which elements of Markdown syntax are — or **are not** — read by three CATs:
- _Wordfast Pro 8_
- _Trados Studio 2022_
- _Phrase_

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
Here we'll see how different types of links are interpreted by *Wordfast Pro*, *Trados Studio 2022*, and _Phrase_.

### Links to Sections with Headers
The link to section on [**Bold** is here](#bold).

### Links to Files
The link to [a Markdown file in the __repository__ is _here_](README.md).

### Links to Images
1. The link to [an image in the **repository** is *here*](images/IMG_20200401_210429.jpg).
2. The link to a displayed image in the repository is here:
   
   ![Shark](images/IMG_20200401_210429.jpg)

3. The link to a displayed image from the internet:
   
   ![Cieszyn](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e2/2012_Powiat_cieszy%C5%84ski%2C_Cieszyn%2C_Rynek%2C_Fontanna_%C5%9Bw._Floriana_02.jpg/310px-2012_Powiat_cieszy%C5%84ski%2C_Cieszyn%2C_Rynek%2C_Fontanna_%C5%9Bw._Floriana_02.jpg "Cieszyn")

### Links to Websites
The link to [my website Translatorion.com is here](https://translatorion.com/).

### Links to YouTube
The link to an embedded David Bowie video on YouTube is here:

[![I am a DJ](http://img.youtube.com/vi/MRRmU_pOXnk/0.jpg)](http://www.youtube.com/watch?v=MRRmU_pOXnk "I am what I play").

### Links with Hover Text

Find a few examples of links with hover text below.

1. The link to section on [**Bold** with a hover text is here](#bold "Bolder").
2. The link to a displayed image in the repository with a hover text is here:

![Shark](images/IMG_20200401_210429.jpg "A Technical Writer Shark")
3. The link to [my website Translatorion.com is here](https://translatorion.com/ "I didn't choose translator's life, translator's life chose me").

### Syntax for Links

Syntax for links — examples:
1. `[**Bold** is here](#bold)`
2. `![Shark](images/IMG_20200401_210429.jpg "A Technical Writer Shark")`
3. `[![I am a DJ](http://img.youtube.com/vi/MRRmU_pOXnk/0.jpg)](http://www.youtube.com/watch?v=MRRmU_pOXnk "I am what I play")`

## Quotations

This section contains various ways of quoting text or code.

### Blockquote

> This is an example of a quote.
>
> > This quote is [inside a quote](https://en.wikipedia.org/wiki/A_Dream_Within_a_Dream "Inception before it was cool").
> > >![inside a quote](./images/deeper.jpg "Deep")
> 
> This quote ~~doesn't~~ *also* include*s* __basic syntax__ and a [*link*](https://en.wikipedia.org/wiki/Link,_West_Virginia).
> 
> — *Confusius*


Syntax:
```
> This is an example of a quote.
>
> > This quote is [inside a quote](https://en.wikipedia.org/wiki/A_Dream_Within_a_Dream "Inception before it was cool").
> > >![inside a quote](./images/deeper.jpg "Deep")
> 
> This quote ~~doesn't~~ *also* include*s* __basic syntax__ and a [*link*](https://en.wikipedia.org/wiki/Link,_West_Virginia).
> 
> — *Confusius*
```

### Inline Code

This is an example of a sentence with an inline code of a text in `**bold** and _italic_`.

Syntax:
```
`**bold** and _italic_`
```

### Code Block

This is an example of code block with Markdown syntax:
```
1. __Bold__
2. *Italic*
   1. ~~Strikethrough~~
3. > Quotation:
   > - unordered list
4. Link [to a very wise person](https://en.wikipedia.org/wiki/Arthur_Schopenhauer)
```
<!-- TUTAJ DODAĆ JESZCZE CYTAT Z JS-->

This is an example of code block with JavaScript syntax:

```js
// This is the code I found somewhere and adapted to another project.
var interval;

function countdown() {
  clearInterval(interval);
  interval = setInterval( function() {
      var timer = $('.js-timeout').html();
      timer = timer.split(':');
      var minutes = timer[0];
      var seconds = timer[1];
      seconds -= 1;
      if (minutes < 0) return;
      else if (seconds < 0 && minutes != 0) {
          minutes -= 0;
          seconds = 40;
      }
      else if (seconds < 10 && length.seconds != 2) seconds = '0' + seconds;

      $('.js-timeout').html(minutes + ':' + seconds);

      if (minutes == 0 && seconds == 0) clearInterval(interval);
  }, 1000);
}

$('#js-startTimer').click(function () {
  $('.js-timeout').text("00:40");
  countdown();
});

$('#js-resetTimer').click(function () {
  $('.js-timeout').text("00:40");
  clearInterval(interval);
});
```

Syntax (part): ` ```js
// This is the code I found somewhere and adapted to another project.
var interval;``` `

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

[^bignote]: Even more additional information

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
<!--- TUTAJ DODAĆ JESZCZE BARDZIEJ ROZWINIĘTĄ PRÓBKĘ TEKSTU --->
**This _sums_ ~~~down~~~ ^up^:**
- ___the `Basic` [Markdown](https://en.wikipedia.org/wiki/Markdown "Cool, innit?") Syntax :sweat_smile:___
- *And all of it in a \*.md file*
- This_is___so__emphatic — this*is***so**emphatic

# HTML and Other Tags
<!-- TUTAJ JESZCZE DAĆ PO PROSTU BLOK KODU HTML GDZIEŚ-->
## General Information

I'll check the following HTML and other tags:
1. [Paragraph](#paragraph)
2. [Code](#code)
3. [Collapsed Section](#collapsed-section)
4. [Keyboard Keys](#keyboard-keys)
5. [Definition](#definition)
6. [Highlight](#highlight-1)
7. [Subscript](#subscript-1)
8. [Superscript](#superscript-1)
9. [Combination of Tags and Markdown Syntax](#combination-of-tags-and-markdown-syntax)
10. [Pure HTML Syntax with JavaScript](#pure-html-syntax-with-javascript)

## Paragraph

<p>**This is *lorem ipsum***: lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur ullamcorper ante sit amet aliquet convallis. Integer mollis urna quis velit mattis facilisis.</p>
<p>Vestibulum pulvinar sed eros vitae eleifend. Mauris et ligula metus. Nunc elementum vestibulum arcu quis ultricies. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.</p>

Syntax: `<p>Lorem ipsum</p>`

==**Note**==: Markdown syntax is ignored in block elements, like `<p></p>` HTML tag.

## Code

This is sample code:
- <code>\<p>Access code: Denied\</p></code>
- <code>**bold** _italic_</code>

Syntax:
- `<code>\<p>Access code: Denied\</p></code>`
- `<code>**bold** _italic_</code>`

==**Note**==: Markdown syntax **is not** ignored in span elements, like `<code></code>` tags.

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

## Keyboard Keys

Use <kbd>W</kbd>, <kbd>S</kbd>, <kbd>A</kbd>, <kbd>D</kbd> keys to move your character in a video game.

And never touch the <kbd>Windows</kbd> key :exploding_head:!

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

*This* is __a combination__ of <mark>various</mark> <kbd>key</kbd> <sup>components</sup> of [Markdown](https://en.wikipedia.org/wiki/Markdown) and <em>HTML</em> <code>tags</code>.

Syntax:
```
*This* is __a combination__ of <mark>various</mark> <kbd>key</kbd> <sup>components</sup> of [Markdown](https://en.wikipedia.org/wiki/Markdown) and <em>HTML</em> <code>tags</code>.
```
## Pure HTML Syntax with JavaScript

<html>
   <head>
      <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
      <style>
         .jotaro {
            background-color: #4f8866;
            padding: 30px;
            border: 5px solid #385A6B;
         }
        .wikkeda {
            font-size: 150%;
            font-family: 'Courier New', Courier, monospace;
            color: #385A6B;
            font-style: italic;
        }
    </style>
   </head>
    <body>
      <div class="jotaro">
         <p class="wikkeda">
            This is an <kbd>HTML</kbd> text with added <a href="https://www.youtube.com/watch?v=F-z6u5hFgPk">styles</a>.
         </p>
         <p>
            This is just a plain <em>HTML</em> text within <code>div</code> style.
         </p>
      </div>
      <div>
         <p>
            This is just a plain <em>HTML</em> text without any style.
         </p>
         <p>
            This is a JavaScript sample that counts down from 40 seconds to 0.
         </p>
         <p>   
            Countdown: <span class="js-timeout">00:40</span>.
         </p>
            <button id="js-startTimer">Start Countdown</button>
            <button id="js-resetTimer">Stop &amp; Reset</button>
            <script src="./timer.js"></script>
      </div>
    </body>
</html>

Syntax:
```html
<html>
   <head>
      <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
      <style>
         .jotaro {
            background-color: #4f8866;
            padding: 30px;
            border: 5px solid #385A6B;
         }
        .wikkeda {
            font-size: 150%;
            font-family: 'Courier New', Courier, monospace;
            color: #385A6B;
            font-style: italic;
        }
    </style>
   </head>
    <body>
      <div class="jotaro">
         <p class="wikkeda">
            This is an <kbd>HTML</kbd> text with added <a href="https://www.youtube.com/watch?v=F-z6u5hFgPk">styles</a>.
         </p>
         <p>
            This is just a plain <em>HTML</em> text within <code>div</code> style.
         </p>
      </div>
      <div>
         <p>
            This is just a plain <em>HTML</em> text without any style.
         </p>
         <p>
            This is a JavaScript sample that counts down from 40 seconds to 0.
         </p>
         <p>   
            Countdown: <span class="js-timeout">00:40</span>.
         </p>
            <button id="js-startTimer">Start Countdown</button>
            <button id="js-resetTimer">Stop &amp; Reset</button>
            <script src="./timer.js"></script>
      </div>
    </body>
</html>
```

## Summary

This sums up combination of `HTML` tags within an `*.md` file.

# Conclusion

I hope this extensive — but definitely not exhaustive — list of Markdown and HTML tags will be a good test for *Wordfast Pro*, *Trados Studio 2022*, and *Phrase*.

I've written this Markdown file in Visual Studio Code that doesn't show the following elements in the preview window:
 - highlight
 - subscript
 - superscript
 - footnotes
 - collapsed section
 - definition
 - JavaScript

Also, not all Markdown syntax or HTML tags work in Github viewer.

# Sources

1. [Markdownguide.org](https://www.markdownguide.org/)
2. [Keyboard glyphs](https://meta.stackexchange.com/questions/5527/keyboard-glyphs)
3. [Collapsed sections](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-collapsed-sections)
4. [Daring Fireball](https://daringfireball.net/projects/markdown/)