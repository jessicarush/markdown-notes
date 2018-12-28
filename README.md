# Markdown Notes

Examples of some of the most common usages. Yes, there are many demos and cheatsheets already out there, but the best way to learn is to do it yourself.

## Table of contents
- [links](#links)
- [headings](#heading-1)
- [code](#code)
- [blockquotes](#blockquotes)
- [line breaks and paragraphs](#line-breaks-and-paragraphs)
- [lists](#lists)
- [text styles](#text-styles)
- [images](#images)
- [horizontal rules](#horizontal-rules)
- [tables](#tables)
- [backslash escapes](#backslash-escapes)
- [TOC Generators](#toc-generators)

## links

As demonstrated above, you can link to any heading within your document using like this: (#lower-case-heading-replace-spaces-with-dashes).

This in an [example link](https://daringfireball.net/projects/markdown/syntax).

You can add the links title attribute like this:
[example link](https://github.com/ "Title goes here")

You can use link references as well:
Here's [Google][1], [Yahoo][2], [MSN][3]

[1]: http://google.com/        "Google"
[2]: http://search.yahoo.com/  "Yahoo Search"
[3]: http://search.msn.com/    "MSN Search"

You can also create automatic links out of a url:
<https://github.com/>


# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6


## code

Here is a block of code:
```
pip3 install mylibrary
```
Here is some `inline code`.

You can also specify syntax highlighting:

```python
print('Python syntax highlighting')
```


## blockquotes

> This is a blockquote
> You can precede each line with > if you're using hard returns.  
> Or if you're soft wrapping you can just add > to the first line.


## line breaks and paragraphs

Two spaces at the end of a line forces a new line.  
Here's my new line.

An empty line creates a new paragraph.

## lists

Unordered lists can be marked with -, +, or *

* point
* point
* point

Ordered lists can be marked with any number.

1. item
1. item
1. item

Task lists:
- [x] This is a complete item
- [ ] This is an incomplete item
- [ ] This is an incomplete item


## text styles

Surround text with single \* or \_ for
*emphasized text*

Surround text with double \*\* or \_\_ for
**strong text**

Surround text with triple \*\*\* for
***strong emphasized text***

Surround text with double \~\~ for
~~strikethrough text~~


## images

![Alt text](img/cat.png)

![Alt text](img/cat.png "Optional title")

You can also place images using the reference method as with links above.


## horizontal rules

Insert a horizontal rule by typing 3 * or - or _ on their own line:

***
___
---


## tables

Use hyphens `-` to indicate header rows and pipes `|` to indicate columns:

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

## TOC Generators

There's a [copy/paste TOC generator](https://ecotrust-canada.github.io/markdown-toc/) for markdown. A better solution is the [installable package on github](https://github.com/jonschlinkert/markdown-toc). Here's a summary of how to get it running:

1. Install the package globally:
```
npm install -g markdown-toc
```

2. In your markdown file, type `<!-- toc -->` where you want the TOC to appear.

3. Run the command to generate the TOC (example filename here is example.md):
```
markdown-toc -i example.md
```

I'm not sure how, but it knows to ignore the headings before `<!-- toc -->`, so for example, if you put a `## Table of Contents` heading before it, it won't get included in the TOC.
