# The Basics

In this section, we present the syntax of Markdown.

## Paragraphs

A paragraph is one or more consecutive lines of text. To create a new paragraph, separate it from the previous paragraph with a blank line. When converting to HTML, the text of the paragraph is wrapped in a **p** tag.

<hr>

### Example:

```
This is a paragraph in Markdown format.
This line will be merged with the previous one.

This is the start of a new paragraph.
```
### Result:

This is a paragraph in Markdown format.
This line will be merged with the previous one.

This is the start of a new paragraph.

<hr>

## Headings

You can specify headings in one of two ways; I'll cover just one of them. To specify that a line
is a heading, start it with a hash mark (#). A heading line can start with 1 to 6 hash marks, corresponding
to HTML's **h1**, **h2**, **h3**, **h4**, **h5**, and **h6** tags.

<hr>

### Example:

```
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```
### Result:

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

<hr>

## Blockquotes

If you need to indicate a quotation in your document, use the notation that has been used in
plain-text e-mail since the dawn of time. That is, start each line with a <q>greater than</q> (>)
symbol. Blockquotes can be nested and can contain other markdown elements.

<hr>

### Example:

```
> # This is a heading inside of a blockquote.
>
> Here's the text of paragraph 1 in the blockquote
>
> > Here's a quote within a quote
>
> Here's the text of paragraph 2 in the blockquote
```
### Result:

> # This is a heading inside of a blockquote.
>
> Here's the text of paragraph 1 in the blockquote
>
> > Here's a quote within a quote
>
> Here's the text of paragraph 2 in the blockquote

<hr>
