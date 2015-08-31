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

## Emphasis

To emphasize a phrase, surround it with asterisks or underscores. If you strongly want to emphasize something, then double the symbols. In HTML, the former will be translated to an **em** tag; the latter as a **strong** tag. By convention, **em** tags appear in *italics* while **strong** tags appear in **bold**.

<hr>

### Example:

```
I *really* want you to be there

No, I _really_ do.

Listen, I **really** want you to be there

I'm __not__ kidding.
```
### Result:

I *really* want you to be there

No, I _really_ do.

Listen, I **really** want you to be there

I'm __not__ kidding.

<hr>

## Lists

You can create two types of lists (just like in HTML). For an unordered list, start each line with an
asterisk (*), a plus (+), or a dash (-), followed by a space and then the content of the list item. For
ordered lists, start each line with a number followed by a period and a space. It doesn't matter what
numbers you use, Markdown will convert it to an HTML ordered list and the browser will take care of
actually numbering the list.

<hr>

### Example:

```
* This is a list

* Items can have

    multiple paragraphs
    if you need them
    just indent by four spaces

    and have blank lines between items

* Here's the end of the list

Here's the start of a new paragraph

1. Here's an ordered list that follows
2. with multiple items
3. as many as you need
```
### Result:

* This is a list

* Items can have

    multiple paragraphs
    if you need them
    just indent by four spaces

    and have blank lines between items

* Here's the end of the list

Here's the start of a new paragraph

1. Here's an ordered list that follows
2. with multiple items
3. as many as you need

<hr>

## Embedded Lists

You can embed one list inside another, as many levels deep as you need (within reason). Just prefix each level
with four spaces in front of the list marker. Level 1 is a normal list. Level 2 lists have four spaces at the
start of their lines. Level 3 lists have eight spaces at the start of their lines, etc.

<hr>

### Example:

```
* This is a list
    * This is an embedded list
        1. that is indicated by adding
        2. four spaces in front of the list marker
    * Go as deep as you need.
* This is the second item of the outer list
* And this is the third item
```
### Result:

* This is a list
    * This is an embedded list
        1. that is indicated by adding
        2. four spaces in front of the list marker
    * Go as deep as you need.
* This is the second item of the outer list
* And this is the third item

<hr>

## Code Elements and Code Blocks

You can have <q>code</q> elements either in-line or in a stand-alone block. In-line code is indicated by surrounding the word or phrase with backticks. Stand-alone code blocks are indicated by four spaces at the start of a line.

<hr>

### Example:

```
Be sure to call the `init()` method before you call `doMyWorkForMe()`.

Also be sure to review this code for me.

    def check(dir: Path) = {
      if (!exists(dir)) {
        error(s"Directory: <$dir> does not exist.")
      }
    }

Thanks!
```

### Result:

Be sure to call the `init()` method before you call `doMyWorkForMe()`.

Also be sure to review this code for me.

    def check(dir: Path) = {
      if (!exists(dir)) {
        error(s"Directory: <$dir> does not exist.")
      }
    }

Thanks!

<hr>




