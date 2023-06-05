General recommendations for translating Markdown
===

# Overview

These general recommendations are for technical writers (or generally, authors writing in Markdown) and translators. The recommendations are not specific for any particular CAT, so they can be used with other CATs as well.

## Recommendations for technical writers

In these recommendations, it is assumed that a technical writer contacts a translator who has little knowledge about Markdown.

- Inform the translator about basic Markdown syntax, because some tags can be shown as text
	NOTE: Feel free to use this [Markdown guide](resources/markdown-basic-intro.md)
- As in writing in general, use simple Markdown formatting — do not combine all possible formatting just to make the text really stand out
- If possible, do not mix Markdown with HTML, JavaScript, JSON, PHP, or similar — put them into separate files
- Brief the translator on the following issues:
	- The scope of translation:
		- Whether comments, inline code, and code blocks need to be translated
		- Whether embedded HTML needs to be translated
		- What must or must not be translated with regard to syntax, e.g. table of contents does not need to be translated if generated automatically, but comments in code blocks may need translation
	- How to view Markdown output files to check if it looks like the source file, nothing is missing, etc.
	- What to do with missing translations if some parts were not imported into the CAT editor, for instance:
		- instruct how to open a Markdown file and how to edit it safely (if the translator has some background knowledge in coding)
		- ask the translator to provide missing translation in a separate text file and enter it on your own in the Markdown output file (if the translator does not have background knowledge in coding; this solution is generally safer)
- Discourage the translator from using machine translation tools because they may translate parts of the code, emojis, and similar content that should not be translated
	- Even if the translator knows Markdown or generally coding, there is still the risk that something will be edited by the machine translation tool and this will not be detected in checks and other quality assurance steps
- Encourage the translator to report:
	- Any characters that are not used in a standard way in the source language as they are most likely tags
	- Any deviations in the output file from the source file
	- Any missing translations in the output file

## Recommendations for translators

In these recommendations, it is assumed that a translator has basic knowledge of Markdown.

- If not briefed by the technical writer, ask the following questions:
	- Do comments, inline code, and code blocks need to be translated?
	- Does embedded HTML need to be translated?
	- Is there anything that requires special care in the Markdown files?
- Choose Markdown filters in the CAT adequately to the source file and the technical writer's brief
- If you have more than one CAT, it may be advisable to try several of them to translate the whole content of the Markdown files
- Do not use machine translation because they may translate parts of the code, emojis, and similar content that should not be translated
	- If machine translation is required by the client or translation agency, pay special attention to code elements because they may have been accidentally edited
- If there are missing translations because the CAT could not import given sections, ask the technical writer:
	- If you are to edit the Markdown files and translate the sections within them
	- If yes, what programs are recommended to open the Markdown files
	- If not, what the preferred method of providing missing translations is (e.g., text files)
- Carefully check the output file in the tool recommended by the technical writer for any missing elements, wrong formatting, etc.
- Immediately contact the technical writer in case of technical problems with the source or output file, or any doubts with the project

---

Go to section: [*Conclusion*](top-conclusion.md)

---

[Back to top](#Overview)
