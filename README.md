# Markdown Notes

Examples of some of the most common usages. I recognize there are many demos and cheatsheets already out there (including the [official markdown guide](https://www.markdownguide.org/basic-syntax/)), but the best way to learn is to do it yourself.

## Table of contents

<!-- toc -->

- [links](#links)
- [headings](#headings)
- [line breaks and paragraphs](#line-breaks-and-paragraphs)
- [blockquotes](#blockquotes)
- [code](#code)
- [lists](#lists)
- [text styles](#text-styles)
- [images](#images)
- [horizontal rules](#horizontal-rules)
- [tables](#tables)
- [backslash escapes](#backslash-escapes)
- [TOC generators](#toc-generators)
- [emoji](#emoji)

<!-- tocstop -->

## links

Link to any heading within your document like this:
```
[Link](#lower-case-heading-replace-spaces-with-dashes)
```

Create an external link like this:
```
[example link](https://daringfireball.net/projects/markdown/syntax)
```
[example link](https://daringfireball.net/projects/markdown/syntax)

You can add the title attribute like this:
```
[example link](https://github.com/ "Title goes here")
```
[example link](https://github.com/ "Title goes here")

You can create link references:
```
[Google][1], [Yahoo][2], [MSN][3]

[1]: http://google.com/        "Google"
[2]: http://search.yahoo.com/  "Yahoo Search"
[3]: http://search.msn.com/    "MSN Search"
```
[Google][1], [Yahoo][2], [MSN][3]

[1]: http://google.com/        "Google"
[2]: http://search.yahoo.com/  "Yahoo Search"
[3]: http://search.msn.com/    "MSN Search"

You can also create automatic links out of a url:
```
<https://github.com/>
```
<https://github.com/>

## headings

Headings can be indicated like:

```
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```


## line breaks and paragraphs

Two spaces at the end of a line forces a new line.  
Here's my new line.

An empty line creates a new paragraph.


## blockquotes

`>` starts a blockquote

> This is a blockquote
> You can precede each line with > if you're using hard returns.  
> Or if you're soft wrapping you can just add > to the first line.


## code

Use single backticks `` ` `` for inline code and triple backticks `` ``` `` for blocks of code.

If the word or phrase you want to denote as code includes one or more backticks, you can escape it by enclosing the word or phrase in double backticks ` `` `.

Here is some `inline code`.

Here is some ``inline `code` with backticks``.

Here is a block of code:
```
pip3 install mylibrary
```

You can also specify syntax highlighting:

```python
print('Python syntax highlighting')
```


## lists

Unordered lists can be marked with `-`, `+`, or `*`

* point
* point
* point

Ordered lists can be marked with any number followed by a period `.`

1. item
1. item
1. item

Task lists can be created using `[ ]` and `[x]`

- [x] This is a complete item
- [ ] This is an incomplete item
- [ ] This is an incomplete item


## text styles

Surround text with single asterisk `*` or underscore `_` for
*emphasized text*

Surround text with double asterisk `**` or underscore `__` for
**strong text**

Surround text with triple asterisk `***` for
***strong emphasized text***

Surround text with double tilde `~~` for
~~strikethrough text~~


## images

```
![Alt text](img/cat.png)
```
![Alt text](img/cat.png)

```
![Alt text](img/cat.png "Optional title")
```
![Alt text](img/cat.png "Optional title")

To add a link to an image, enclose the Markdown for the image in brackets, and then add the link in parentheses.

```
[![Alt text](img/cat.png "Optional title")](img/cat.png)
```
[![Alt text](img/cat.png "Optional title")](img/cat.png)


## horizontal rules

Insert a horizontal rule by typing three or more `*` or `-` or `_` on their own line. For compatibility, put blank lines before and after horizontal rules.

```
***

___

---
```

***

## tables

Use hyphens `-` to indicate header rows and pipes `|` to indicate columns:

```
id | name | email
-- | ---- | -----
1 | rick | rick@email.com
2 | morty | morty@email.com
```
id | name | email
-- | ---- | -----
1 | rick | rick@email.com
2 | morty | morty@email.com


## backslash escapes

Markdown provides backslash escapes for the following characters:

```
\   backslash
`   backtick
*   asterisk
_   underscore
{}  curly braces
[]  square brackets
()  parentheses
#   hash mark
+   plus sign
-   minus sign (hyphen)
.   dot
!   exclamation mark
```

## TOC generators

There's a [copy/paste TOC generator](https://ecotrust-canada.github.io/markdown-toc/) for markdown. A better solution is the [installable package on github](https://github.com/jonschlinkert/markdown-toc). Here's a summary of how to get it running:

1. Install the package globally:
```
npm install -g markdown-toc
```

2. In your markdown file, type:

  ```
  <!-- toc -->

  <!-- tocstop -->
  ```

  Headings that appear before this will not be included. For example, if you put a `## Table of Contents` heading before it, this won't get included in the toc.

## emoji

You can insert most emoji characters using the following syntax:

:warning: `:warning:`  
:exclamation: `:exclamation:`  
:question: `:question:`  
:grey_exclamation: `:grey_exclamation:`  
:grey_question: `:grey_question:`  
:star: `:star:`  
:speech_balloon: `:speech_balloon:`  
:thought_balloon: `:thought_balloon:`  
:bulb: `:bulb:`  
:clipboard: `:clipboard:`  
:pencil2: `:pencil2:`  
:x: `:x:`  

This can be combined with the blockquote syntax to make something like an admonition:

> :warning: Attention: this is not as good as a reStructuredText admonition

An extensive list of markdown emoji can be found here:
<https://gist.github.com/rxaviers/7360908>
