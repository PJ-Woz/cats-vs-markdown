---
title: Why is Markdown difficult for CATs?
layout: default
nav_order: 3
parent: Overview
---
# Why is Markdown difficult for CATs?

Because Markdown syntax uses characters that can appear in a text in their normal use and there are different characters that serve the same purpose, it is difficult for CAT software developers to create good Markdown filters. The filters need to sift out Markdown tags and place non-editable tags in a CAT program. The tags in the CAT must be non-editable to avoid accidental editing or deletion.

However, some Markdown tags must be editable to a certain degree:

```
1. Hello ***.md** my old friend!
2. ![Shark](resources/images/IMG_20200401_210429.jpg "A Technical Writer Shark")
```

In the first example, `**` is a tag for **bold**. We do not want the CAT to interpret it as two asterisks because they may be accidentally changed or deleted. As a result, the CAT should place a non-editable opening [tag](glossary#cat,-tag) where the text in bold starts and a closing tag where the text in bold ends. However, we **do** want the one asterisk to be shown normally.

In the second example, the whole line is a reference to a displayed image file with a hover text `A Technical Writer Shark`. In this case, we want the CAT to interpret `Shark` and `A Technical Writer Shark` as translatable, but leave the brackets and link to the image file as non-translatable.

That is why the difficulty lies in using such filters that interpret asterisks or brackets as Markdown tags, while also interpret them as normal characters used in the text. This is made difficult even further when combined with other characters that build up Markdown tags.

# Fringe cases for translation Markdown

There are cases that we may — or may not — want to translate some content within Markdown tags, namely:

- links reference:
	`[**Bold**](#bold)`, which is a link to a section with a header "Bold"
	There may be cases where this is not necessary, like in a table of contents, which can be generated automatically

- inline code:

```
1. This is what a link to the section on `[**Bold**](#bold)` looks like.
2. HTML syntax for links is as follows: `<a href="www.google.com">Google</a>.`
```

In the first example, we may want to translate the content of the inline code, while in the second example, we may want to ignore it to prevent accidental editing.

- code block:
```
	```
	<script>
	function myFunction() {
	  document.getElementById("demo").innerHTML = "Paragraph changed.";
	}
	</script>
	```
```

In this example, the use case may be to leave the whole code block as non-translatable. However, if the variables are to be translated as well, then the code block must be imported into the CAT editor.

- comments:
```markdown
1. This is a section on **bold**. <!-- Please write below your own examples. -->
2. # The one and only Markdown guide you'll ever need  <!-- Marketing said we needed a more flashy header -->
```

In this example, there is a need to translate the comment as it contains an instruction for the reader. In the second example, the comment does not have to be translated if it is an internal comment in an English speaking team.

# The CATs and testing Markdown

Markdown filters in Phrase, Trados Studio 2022, and Wordfast Pro 8 were tested on various Markdown tags in different combinations. A special test file was created for this purpose.

---

Next section: [*The test file*](ref-test-file)