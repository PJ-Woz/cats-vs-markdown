An Introduction to Markdown in Standard Technical English<!-- omit in toc -->
===
 

## Table of Contents<!-- omit in toc -->

- [Markdown - Introduction](#markdown---introduction)
- [Line Break](#line-break)
  - [What is Line Break?](#what-is-line-break)
  - [How to Create Line Break](#how-to-create-line-break)
- [Bold](#bold)
  - [What is Bold?](#what-is-bold)
  - [How to Create Text in Bold](#how-to-create-text-in-bold)
- [Italic](#italic)
  - [What is Italic?](#what-is-italic)
  - [How to Create Text in Italic](#how-to-create-text-in-italic)
- [Header](#header)
  - [What is a Header?](#what-is-a-header)
  - [How to Create a Header](#how-to-create-a-header)
- [Link](#link)
  - [What is a Link?](#what-is-a-link)
  - [How to Create a Link](#how-to-create-a-link)
- [Quotation](#quotation)
  - [What Is a Quotation?](#what-is-a-quotation)
  - [How to Create a Quotation](#how-to-create-a-quotation)
- [List](#list)
  - [Bullet List](#bullet-list)
    - [What is a Bullet List?](#what-is-a-bullet-list)
    - [How to Create a Bullet List](#how-to-create-a-bullet-list)
  - [Numbered List](#numbered-list)
    - [What Is Numbered List?](#what-is-numbered-list)
    - [How to Create a Numbered List](#how-to-create-a-numbered-list)
- [Tables](#tables)
  - [What Is a Table?](#what-is-a-table)
  - [How to Create a Table](#how-to-create-a-table)
- [Conclusion](#conclusion)


# Markdown - Introduction

In this simple introduction, you will learn the basics of Markdown language. You will need about two hours to learn the basics.

# Line Break  

## What is Line Break?

A "line break" creates paragraphs in your text.

## How to Create Line Break

Use the following methods to create paragraphs with line breaks:
- Press the <kbd>ENTER</kbd> key twice at the end of the paragraph
- Press the <kbd>SPACE BAR</kbd> twice. Then, press the <kbd>ENTER</kbd> key

# Bold

## What is Bold?

"Bold" creates a text, which is highglighted with **thick** letters.

## How to Create Text in Bold

Use the asterisk "\*\*" or underline "\_\_" symbols around the text which you want to highlight in bold:
- `**formatted text**`
- `__formatted text__`

# Italic

## What is Italic?

"Italic" creates a text, which is highlighted with *slanted* letters.

## How to Create Text in Italic

Use the asterisk "*" or underline "_" symbols around the text which you want to highlight in italic:
- `*formatted text*`
- `_formatted text_`

# Header

## What is a Header?

A "header" is a title of a section. There are six types of headers. Each type of the header is in a different size.

## How to Create a Header

Use the hash symbol "#" to create a header. To create a header in smaller size, use the symbol more times:
- `# Title size 1`
- `## Title size 2`
- `### Title size 3`
- `#### Title size 4`
- `##### Title size 5`
- `###### Title size 6`

Press the <kbd>ENTER</kbd> key twice at the end of the header to finish the title.

# Link

## What is a Link?

A "link" is a function to send you to other objects. The objects can be:
- A website on the Internet
- A file in a GitHub repository
- An image in a GitHub repository
- An image on the Internet
- A header in the current text

## How to Create a Link

A link needs two elements to work:
1. The text of the link
2. The address of the object you want to link to

The text of the link is placed in square brackets. Square brackets are "[" and "]".

The address of the object you want to link to is placed in rounded brackets. Rounded brackets are "(" and ")".

Use the following combinations of texts and addresses to create links:
- a website on the Internet: `[Text](Internet address)`
- a file in a GitHub repository: `[Text](address to the file in a GitHub repository)`
- an image in a GitHub repository: `[Text](address to the image file in a GitHub repository)`
  - :bulb:Note: if you want to display your image, use an exclamation mark "!" in front of the square brackets. It looks like this: `![Text](address to the image file in a GitHub repository)`
- an image on the Internet: `[Text](address to the image file on the Internet)`
  - :bulb:Note: if you want to display your image, use an exclamation mark "!" in front of the square brackets. It looks like this: `![Text](address to the image file on the Internet)`
- a header in the current text: `[Text](address to the header in the current text)`

You can find examples of the code for links below:
- a website on the Internet: `[Translatorion](https://translatorion.com/language/en/translatorion/)`
- a file in a GitHub repository: `[A Markdown Text](/Praca-2022-11-20.md)`
- an image in a GitHub repository: `[Shark](/Images/IMG_20200401_210429.jpg)`
  - :bulb:Note: if you want to display your image, use an exclamation mark "!" in front of the square brackets. It looks like this: `![Shark](/Images/IMG_20200401_210429.jpg)`
- an image on the Internet: `[Cieszyn](https://upload.wikimedia.org/wikipedia/commons/thumb/5/58/Cieszyn_Rynek2.jpg/1280px-Cieszyn_Rynek2.jpg)`
  - :bulb:Note: if you want to display your image, use an exclamation mark "!" in front of the square brackets. It looks like this: `![Cieszyn](https://upload.wikimedia.org/wikipedia/commons/thumb/5/58/Cieszyn_Rynek2.jpg/1280px-Cieszyn_Rynek2.jpg)`
- a header in the current text: `[How to Create a Link](#how-to-create-a-link)`

# Quotation

## What Is a Quotation?

A "quotation" is a direct reference to some other piece of text. For example, a quotation can be words of a famous person, a section of a text, a part of programming code, or a section of programming code.

## How to Create a Quotation

Use the following symbols to create a quotation:
- Use the more-than symbol ">" to create a quotation of a section of a text: `> Text`
- Use a backtick symbol "\`" to create a quotation of a part of programming code: <code>\`\*italic*\`</code>
- Use a backtick symbol "\`" three times to create a quotation of a section of programming code:
<code>
\```
\# A Sample Header
\```
</code>

# List

## What is a List?

A "list" is an arrangement of items one under another.

There are two types of lists:
- [Bullet List](#bullet-list)
- [Numbered List](#numbered-list)

## Bullet List

### What is a Bullet List?

A "bullet list" is an arrangement of items one under another. The order of items in a bullet list is not important. The order of items does not create a sequence.

### How to Create a Bullet List

Use the minus symbol "-" to create a bullet list. To add another item to the bullet list, press the <kbd>ENTER</kbd> key. Then, use the minus symbol "-" again like in the example below:
```
- Item
- Item
- Item
```
:bulb:Note: many Markdown editors add the minus symbol "-" automatically when you press the <kbd>ENTER</kbd> key.

:bulb:Note: press the <kbd>TAB</kbd> key in front of the minus symbol "-" to create an indent in the bullet list.

## Numbered List

### What Is Numbered List?
A "numbered list" is an arrangement of items one under another. The order of items is important. The order of items creates a sequence.

### How to Create a Numbered List
Use digits from the set of `{1, 2, 3, 4, 5, 6, 7, 8, 9, 0}` to create numbers on the numbered list. Place a full stop "." after the number. To add another item to the numbered list, press the <kbs>ENTER</kbd> key. Then, use digits from the set of `{1, 2, 3, 4, 5, 6, 7, 8, 9, 0}` to create the subsequent number on the numbered list like in the example below:
```
1. Item 1
2. Item 2
3. Item 3
```
:bulb:Note: many Markdown editors add the subsequent number automatically when you press the <kbd>ENTER</kbd> key.

:bulb:Note: press the <kbd>TAB</kbd> key in front of the number to create indent in the numbered list.

# Tables

## What Is a Table?
A "table" is an arrangement of data in rows and columns. One block on the intersection of a row and a column is called a "cell".

## How to Create a Table
To create a table, you use two symbols. The first symbol is vertical bar "|". The second symbol is the minus symbol "-".

To create a table:
1. Use the vertical bar symbol to open a cell
2. Type the content of the cell
3. Use the vertical bar symbol to close the cell
   - :bulb:Note: this cell will create the first column in the first row
4. Repeat steps 2-3 to create as many cells as needed
5. Press the <kbd>ENTER</kbd> key
6. Use the vertical bar symbol to open a cell
7. Type three minus symbols
8. Use the vertical bar symbol to close the cell
9. Repeat steps 7-8 as many times as there are cells in the first row
10. Press the <kbd>ENTER</kbd> key to create another row
11. Repeat steps 1-5 to create as many rows as needed
12. Press the <kbd>ENTER</kbd> key twice to close the table

A code for a sample table looks as follows:
```
| Text | Text   | Text      | Text |
| --- | --- | --- | --- |
| Text  | Text | Text      | Text  |
| Text  | Text | Text | Text  |
```

# Conclusion

You have covered Markdown basics.

To create texts in Markdown, you can use, for example, [Visual Studio Code](https://code.visualstudio.com/) software.