# Syntax #

Using Markua[^markua-spec] flavor of Markdown with some enhancements to improve workflow and extend usage beyond just books.

[^markua-spec]: Armstrong, Peter. 2014. The Markua Specification. Leanpub. https://leanpub.com/markua

# Text Formatting

How to format text

## Italicized or Emphasized Text

```
This is *italicized text* using an asterisk.
```

Output: This is *italicized text* using an asterisk.

The single * syntax maps to \<em> tag in HTML and is used to convey semantic emphasis, which is almost always styled with italics.

```
This is _italicized text_ using an underscore.
```

Output: This is _italicized text_ using an underscore.

The single _ syntax maps to \<i> tag in HTML and is used for italic styling only (does not convey semantic meaning).

## Bold or Strong Text

```
This is **bold text** using two asterisks.
```

Output: This is **bold text** using two asterisks.

The double ** syntax maps to \<strong> tag in HTML is used to convey semantic strong importance, which is almost always styled as boldface.

```
This is __bold text__ using two underscores.
```

Output: This is __bold text__ using two underscores.

The double __ syntax maps to \<b> tag in HTML and is used for bold styling only (does not convey semantic meaning).

## Bold Italicized or Strong Emphasized Text

```
This is ***bold italicized text*** using three asterisks.
```

Output: This is ***bold italicized text*** using three asterisks.

The triple *** syntax maps to \<strong>\<em> tags in HTML is used to convey semantic strong importance with emphasis, which is almost always styled as boldface and italics.

```
This is ___bold italicized text___ using three underscores.
```

Output: This is ___bold italicized text___ using three underscores.

The triple ___ syntax maps to \<b>\<i> tags in HTML and is used for bold italic styling only (does not convey semantic meaning).

## Underlined Text

```
This is ****underlined text**** using four asterisks.
```

Output: This is ****underlined text**** using four asterisks.

The quadruple **** syntax maps to \<u> tag in HTML is used for underline styling.

```
This is ____underlined text____ using four underscores.
```

Output: This is ____underlined text____ using four underscores.

The quadruple ____ syntax maps to \<u> tag in HTML is used for underline styling.

## Bold, Italic, and Underline Summary

<!-- This is how complex tables are specified in Markua, but my Markdown converter doesn't support right now
|:================================:|:=============================================:|:=================:|
| Markua Syntax                    | HTML Produced                                 | Appearance        |
|:=================================|:==============================================|:==================|
| \_one underscore\_               | \<i>one underscore\</i>                       | _italic_          |
|----------------------------------|-----------------------------------------------|-------------------|
| \*one asterisk\*                 | \<em>one asterisk\<em>                        | *italic*          |
|----------------------------------|-----------------------------------------------|-------------------|
| \_\_two underscores\_\_          | \<b>two underscores</b>                       | __bold__          |
|----------------------------------|-----------------------------------------------|-------------------|
| \*\*two asterisks\*\*            | \<strong>two asterisks/<strong>               | **bold**          |
|----------------------------------|-----------------------------------------------|-------------------|
| \_\_\_three underscores\_\_\_    | \<b>\<i>three underscores\</i>\</b>           | ___bold italic___ |
|----------------------------------|-----------------------------------------------|-------------------|
| \*\*\*three asterisks\*\*\*      | \<strong>\<em>three asterisks\</em>\</strong> | ***bold italic*** |
|----------------------------------|-----------------------------------------------|-------------------|
| \_\_\_\_four underscores\_\_\_\_ | \<u>four underscores\</u>                     | ____underline____ |
|----------------------------------|-----------------------------------------------|-------------------|
| \*\*\*\*four asterisks\*\*\*     | \<u>four asterisks\</u>                       | ****underline**** |
|----------------------------------|-----------------------------------------------|-------------------|
-->


| Markua Syntax                    | HTML Produced                                 | Appearance        |
|----------------------------------|-----------------------------------------------|-------------------|
| \_one underscore\_               | \<i>one underscore\</i>                       | _italic_          |
| \*one asterisk\*                 | \<em>one asterisk\<em>                        | *italic*          |
| \_\_two underscores\_\_          | \<b>two underscores</b>                       | __bold__          |
| \*\*two asterisks\*\*            | \<strong>two asterisks/<strong>               | **bold**          |
| \_\_\_three underscores\_\_\_    | \<b>\<i>three underscores\</i>\</b>           | ___bold italic___ |
| \*\*\*three asterisks\*\*\*      | \<strong>\<em>three asterisks\</em>\</strong> | ***bold italic*** |
| \_\_\_\_four underscores\_\_\_\_ | \<u>four underscores\</u>                     | ____underline____ |
| \*\*\*\*four asterisks\*\*\*     | \<u>four asterisks\</u>                       | ****underline**** |


## Strikethrough

```
This is ~~strikethrough~~ test using two tildes.
```

Output: This is ~~strikethrough~~ test using two tildes.

## Superscript

```
This is ^superscript^ surrounded with 
carets.
```

Output: This is ^superscript^ surrounded with carets.

## Subscript

``` 
This is ~subscript~ surrounded with tildes.
```

Output: This is ~subscript~ surrounded with tildes.

# Headings

```
# Part #
```

```
# Chapter
```

```
## Section
```

```
### Sub-Section
```

```
#### Sub-Sub-Sub Section
```

```
##### Sub-Sub-Sub-Sub Section
```

```
###### Sub-Sub-Sub-Sub-Sub Section
```

# Spaces, Newlines, and Indentations

## Paragraphs

```
I'm paragraph one.

I'm paragraph two.

I'm paragraph three. 
I'm still paragraph three. 
```

## Line Breaks

```
A forced line
break in input
is a force line break in 
output
```

A forced line
break in input
is a force line break in 
output


## Leading Spaces

Following **exactly one** newline, whitespace is **preserved**.

Following **two or more** newlines, whitespace is **ignored**.

## Trailing Spaces

All trailing spaces at the end of a line are ignored

## Internal Spaces

```
Spaces or tabs      in the middle        of a line are     collapsed to a single space.
```

Spaces or tabs      in the middle        of a line are     collapsed to a single space.

# Resources

Resources vary in four different ways:

1. **Insertion Methods**: Span and Figure
2. **Locations**: Local, Web and Inline
3. **Types**: image, video, audio, code or math
4. **Formats**: `png`, `m4a`, `mp3`, `ruby`, `latex`, `plain`, etc.

There are five types of resources: image, video, audio, code and math. Each type of resource has a number of supported formats. Any of the five resource types can be inserted as a local resource or web resource, and many of the resource types can also be inserted as an inline resource.

## Figures


The syntax for a local resource or a web resource inserted as a figure is as follows:

~~~
{key: value, comma: separated, optional: attribute_list}
![Optional Figure Caption](resource_path_or_url)
~~~

The syntax for an inline resource inserted as a figure is as follows:

~~~
{key: value, comma: separated, optional: attribute_list}
```optional_format
inline resource content (default format is `guess`)
```
~~~

### Figure Attributes

A figure can also have attributes. The supported attributes vary based on the type of resource, but all figures support the `format`, `caption` and `class` attributes.

`format`
: This is the resource format. Different resource types have different legal values for format.

`caption`
: This is text which is shown near the figure, typically above or below it. A Markua Processor can choose where to position captions based on any criteria it chooses. For example, a Markua Processor can position all captions above or below figures, or use a different behaviour based on the resource format.

`class`
: Any attribute list supports a class attribute. When used in figures, this is the class of the figure. This can be used for styling, and it can also be used by Markua Processors which wish to group figures by classes (e.g. theorems, lemmas, etc).


### Figure Captions


The caption for a figure can be provided either in the square brackets in front of a local or web resource or in the attribute list above the resource:

~~~
![My Amazing Algorithm](algorithm.rb)

{caption: "My Amazing Algorithm}
![](algorithm.rb)
~~~

### Figure Alt Text

The alt text should **not** have the same content as the figure caption, if the figure caption is present. (Imagine the annoyance of having a visual disability and having your screen reader read identical alt text and figure captions to you throughout an entire book!) Instead, the alt text should be descriptive of the image content.

These are some examples of figures with both alt text and a figure caption:

~~~
{alt: "Denzel Washington on a jet ski in a river"}
![Washington Crossing the Delaware](delaware.jpg)

{alt: "Denzel Washington on a jet ski in a river", caption: "Washington Crossing the Delaware"}
![](delaware.jpg)

{caption: "Earth From Space (Simplified)", alt: "a blue circle"}
```svg
<svg width="20" height="20">
  <circle cx="10" cy="10" r="9" fill="blue"/>
</svg>
```
~~~

### Spans (Single Backticks)

Two types of resources can be inserted as inline spans: code resources of format `text`, and math resources of format `latex`.

An inline code resource of `text` format can be inserted as a span using the following syntax:

~~~
It's a single backtick `followed by inline resource content` and then a single backtick.
~~~

An inline math resource of `latex` format can be inserted as a span using the following syntax:

~~~
It's a single backtick `followed by inline resource content`$ and then a single backtick and dollar sign.
~~~

### Figures That Look Like Spans

The following two paragraphs are equivalent:

~~~
Here's some text ![Foo](bar.png) and more text.

Here's some text
![Foo](bar.png)
and more text.
~~~

## Resource Locations

A resource is either considered a local, web or inline resource based on its location:

Local Resource
: The resource is stored in a `resources` directory on a local filesystem (or one of it's subdirectories)

Web Resource
: The resource is referred to via an `http` or `https` URL.

Inline Resource
: The resource is defined right in the body of the document.

### Local Resource

A file called `foo.jpg` in the `resources` directory is referenced as `![](foo.jpg)`--not as `![](/foo.jpg)`, `![](resources/foo.jpg)` or  `![](/resources/foo.jpg)`.

A file called `bar.png` in a subdirectory `images` of the resources directory is referenced as `![](images/bar.png)`--not as `![](/images/bar.png)`, `![](resources/images/bar.png)` or  `![](/resources/images/bar.png)`.


### Web Resources

Web resources are identified by the absolute URL of the resource on the internet. In the case of image, audio and video resources, this becomes the `src` attribute of the resource in HTML.

### Inline Resources

Inline resources can be of type code or math (regardless of format) and they can also be image resources of `svg` format.

## Resource Types and Formats

There are five types of resources: image, video, audio, code, and math. Each type of resource has a number of supported formats. The format determines the type.

{caption: "Formats Mapped to Resource Types"}

| Format Detected                     | Resource Type Inferred |
|-------------------------------------|------------------------|
| `gif`, `png`, `jpeg`, `svg`, `svgz` | image                  |
| `mp4`, `webm`                       | video                  |
| `mp3`, `aac`, `wav`, `ogg`          | audio                  |
| `latex`, `mathml`                   | math                   |
| `text`, `guess` (unrecognized)      | code                   |



### Images

Images are always inserted as figures. 

Images can have the following attributes:
* alt
* caption
* class
* format
* cite
* url

For example:

```
{alt: "a slice of chocolate cake", cite: "Peter Armstrong's Food Photography", url: "http://peterarmstrong.com/pictures/1.jpg"}
![A Piece of Cake](cake.jpg)
```

### Video

Videos can have the following attributes:
* format (mp4, webm)
* poster (URL or path to image displayed before video is played
* caption
* class

For example:

```
{poster: http://img.youtube.com/vi/VOCYL-FNbr0/mqdefault.jpg}
![Introducing Markua](https://www.youtube.com/watch?t=105&v=VOCYL-FNbr0)
```

### Audio

Audio can have the following attributes:
* format (mp3, acc, wav, ogg)
* caption
* class

For example:
```
![Full Talk](http://markua.com/talk.m4a)
```

### Code

Code can have the following attributes:
* caption
* class
* format (name of programming language)
* line-numbers (true or false)
* number-from (default is 1)
* crop-start
* crop-end

For example: 
```
{format: ruby}
![Hello World in Ruby](hello.rb)
```

Another example:
~~~
{format: ruby}
```
puts "hello"
```
~~~


Inline code resource: 
```
Yada yada `some code here` yada yada.
```

### Math

Math resources can be either LaTeX math or MathML.

Math can  have the following attributes:
* alt
* caption
* class
* format (latex, mathml)

For example:
```
{alt: "too large to fit in the alt text"}
![Proof of Fermat's Last Theorem](fermat_proof.mathml)
```

Another example:
```
{alt: "too large to fit in the alt text"}
![Proof of Fermat's Last Theorem](http://markua.com/fermat_proof.tex)
```

Inline example:
```
Yada yada `some math here`{format: latex} yada yada.
```

# Lists

Ordered (numbered), unordered (bulleted), and definition lists are supported. 

## Unordered Lists (Bulleted Lists)

Build a list out of items starting with an asterisk and one space:

~~~
* foo
* bar
* baz
~~~

Output:
* foo
* bar
* baz

## Ordered Lists (Numbered Lists)

An ordered list can vary the following:

1. Numbering system
2. Numbering direction (ascending or descending)
3. Initial number (or letter, or Roman numeral)

The following choices of numbering system are supported:

1. Decimal numbers
2. Uppercase letters
3. Lowercase letters
4. Uppercase Roman numerals
5. Lowercase Roman numerals


Ascending decimal numbers starting from 1:

~~~
1. foo
2. bar
3. baz
~~~

Output: 
1. foo
2. bar
3. baz

Ascending decimal numbers starting from a higher number:

~~~
9.  foo
10. bar
11. baz
~~~

Output:
9.  foo
10. bar
11. baz

Descending decimal numbers:

~~~
3. foo
2. bar
1. baz
~~~

Output: 
3. foo
2. bar
1. baz

Ascending lowercase letters:

~~~
a. foo
b. bar
c. baz
~~~

Output:
a. foo
b. bar
c. baz

Ascending uppercase letters:

~~~
I. foo
J. bar
K. baz
~~~

Output:
I. foo
J. bar
K. baz

Ascending uppercase Roman numerals:

~~~
I.   foo
II.  bar
III. baz
~~~

Output:
I.   foo
II.  bar
III. baz


## Nested Lists

There is a limit of **three** levels of nesting.

Use **two** spaces to indicate a nested level.

~~~
* Foo
  1. One
  2. Two
    a. This is 2a
    b. This is 2b
  3. Three
* Bar
  i.   Lorem
  ii.  Ipsum
  iii. Dolor
* Baz
~~~

Output:
* Foo
  1. One
  2. Two
    a. This is 2a
    b. This is 2b
  3. Three
* Bar
  i.   Lorem
  ii.  Ipsum
  iii. Dolor
* Baz

## Definition Lists

There can be one to three spaces after the colon, or one tab.

Example definition list:

~~~
term 1
: definition 1a
: definition 1b

term 2
: definition 2
~~~

Output:
term 1
: definition 1a
: definition 1b

term 2
: definition 2


# Tables

There are two ways to create tables: simple and complex.

## Simple Tables

At its most basic, a simple table looks like this:

~~~
Header A   | Header B   | Header C
-----------|------------|-----------
Content A1 | Content B1 | Content C1
Content A2 | Content B2 | Content C2
Content A3 | Content B3 | Content C3
~~~

Output:
Header A   | Header B   | Header C
-----------|------------|-----------
Content A1 | Content B1 | Content C1
Content A2 | Content B2 | Content C2
Content A3 | Content B3 | Content C3

You can also start and end the columns with pipes:

~~~
| Header A   | Header B   | Header C   |
|------------|------------|------------|
| Content A1 | Content B1 | Content C1 |
| Content A2 | Content B2 | Content C2 |
| Content A3 | Content B3 | Content C3 |
~~~

Output:
| Header A   | Header B   | Header C   |
|------------|------------|------------|
| Content A1 | Content B1 | Content C1 |
| Content A2 | Content B2 | Content C2 |
| Content A3 | Content B3 | Content C3 |

Finally, you can specify left, center and right alignment of columns with colons in the header separator row. The following columns are left-, center-, and right-aligned respectively:

~~~
| Header A    | Header B     | Header C    |
|:------------|:------------:|------------:|
| Content A1  | Content B1   | Content C1  |
| Content A2  | Content B2   | Content C2  |
| Content A3  | Content B3   | Content C3  |
~~~

Output:
| Header A    | Header B     | Header C    |
|:------------|:------------:|------------:|
| Content A1  | Content B1   | Content C1  |
| Content A2  | Content B2   | Content C2  |
| Content A3  | Content B3   | Content C3  |

## Complex Tables

At its most standard, a complex table looks like this:

~~~
|============|============|============|
| Header A   | Header B   | Header C   |
|============|============|============|
| Content A1 | Content B1 | Content C1 |
|------------|------------|------------|
| Content A2 | Content B2 | Content C2 |
|------------|------------|------------|
| Content A3 | Content B3 | Content C3 |
|============|============|============|
| Footer A   | Footer B   | Footer C   |
|============|============|============|
~~~

Output:
|============|============|============|
| Header A   | Header B   | Header C   |
|============|============|============|
| Content A1 | Content B1 | Content C1 |
|------------|------------|------------|
| Content A2 | Content B2 | Content C2 |
|------------|------------|------------|
| Content A3 | Content B3 | Content C3 |
|============|============|============|
| Footer A   | Footer B   | Footer C   |
|============|============|============|


You can individually align cells with colons in the `-` part-row **above** them. This alignment overrides any alignment already on the column, and it works for merged cells too:

~~~
|=============|===============|=============|
| Header A    | Header B      | Header C    |
|:============|:=============:|============:|
| Content A1 and B1 Merged    | Content C1  |
|------------:|:--------------|-------------|
| Content A2  | Content B2    | Content C2  |
|:-----------:| and B3 Merged |-------------|
| Content A3  |               | Content C3  |
|=============|===============|=============|
| Footer A    | Footer B      | Footer C    |
|=============|===============|=============|
~~~

Output:
|=============|===============|=============|
| Header A    | Header B      | Header C    |
|:============|:=============:|============:|
| Content A1 and B1 Merged    | Content C1  |
|------------:|:--------------|-------------|
| Content A2  | Content B2    | Content C2  |
|:-----------:| and B3 Merged |-------------|
| Content A3  |               | Content C3  |
|=============|===============|=============|
| Footer A    | Footer B      | Footer C    |
|=============|===============|=============|

## Table Captions and Attributes

Supported attributes for tables:
* caption
* class

# Block Elements

Here are more block elements beyond the paragraphs, headings, and figures already described.

## Scene Breaks

To make a scene break, create a line which has only hyphens, asterisks, or underscores. There must be a blank line above and below. 

Example:

~~~
This is before the first scene break.

* * *

This is after the first scene break and before the second.

---

This is after the second scene break.
~~~

Output:
This is before the first scene break.

* * *

This is after the first scene break and before the second.

---

This is after the second scene break.

## Blockquotes (>)


Blockquotes in Markua are created in one of two ways:

1. By prefacing lines with `> `, i.e. a greater than character followed by a space.
2. By wrapping the blockquote in `{blockquote}` ... `{/blockquote}`

Example:
~~~
This is the first paragraph.

> This is a blockquote.
>
> It is outside the paragraphs.

This is the second paragraph.
~~~

Output: 
This is the first paragraph.

> This is a blockquote.
>
> It is outside the paragraphs.

This is the second paragraph.

Blockquote with citation:
~~~
{cite: "Marc Andreessen", url: "http://www.wsj.com/articles/SB10001424053111903480904576512250915629460"}
> Software is eating the world.
~~~

Output:
{cite: "Marc Andreessen", url: "http://www.wsj.com/articles/SB10001424053111903480904576512250915629460"}
> Software is eating the world.


## Asides (A>)

Typically short or long notes which are tangential to the main idea.

The syntaxes for asides are very similar to blockquotes:

1. By prefacing lines with `A> `
2. By wrapping the aside in `{aside}` ... `{/aside}`

Here's a short aside:

~~~
A> This is a short aside.
~~~

Output:
A> This is a short aside.

Here's a longer aside, which also contains a heading:

~~~
A> # A Longer Aside
A>
A> This is a longer aside.
A>
A> It can have multiple paragraphs.
A>
A> The `A> ` stuff can get tedious after a while.
A>
A> This is why the `{aside}` syntax exists.
~~~

Output:
A> # A Longer Aside
A>
A> This is a longer aside.
A>
A> It can have multiple paragraphs.
A>
A> The `A> ` stuff can get tedious after a while.
A>
A> This is why the `{aside}` syntax exists.


## Blurbs (>B)

Blurbs are like asides, but shorter. 

The syntaxes for blurbs are very similar to asides:

1. By prefacing lines with `B> `
2. By wrapping the blurb in `{blurb}` ... `{/blurb}`

Examples:

~~~
B> This is a short blurb.
~~~

Output:
B> This is a short blurb.

~~~
B> # A Longer Blurb
B>
B> This is a longer blurb.
B>
B> It can have multiple paragraphs.
~~~

Output:
B> # A Longer Blurb
B>
B> This is a longer blurb.
B>
B> It can have multiple paragraphs.


Supported attributes for blurbs:
* class (discussion, error, exercise, information, question, tip, warning)
* icon (references an icon from Font Awesome)

Examples:

~~~
{class: warning}
B> This is a warning!
~~~

Output:
{class: warning}
B> This is a warning!

~~~
{icon: car}
B> You can't spell carbon without it!
~~~

Output:
{icon: car}
B> You can't spell carbon without it!

# Span Elements

Here are more span elements beyond the resources already described.

## Links



### Inline Links

The normal way to create a link is as follows:

~~~
[link text](absolute_url)
~~~

Example:

~~~
Markua was developed at [Leanpub](http://leanpub.com).
~~~

Output:
Markua was developed at [Leanpub](http://leanpub.com).


### Automatic Links

To create a link where the text displayed for the link text is the URL itself, the automatic link syntax can be used. 

~~~
Some text <absolute_url> some text.
~~~

Example:

~~~
Markua was developed at <http://leanpub.com>.
~~~

Output:
Markua was developed at <http://leanpub.com>.


### Span Attributes

Surrounding text in square brackets adds attributes to an arbitrary span of text:

~~~
Some text [then a span]{and: an, attribute: list} attached to the span.
~~~

Output:
Some text [then a span]{and: an, attribute: list} attached to the span.

## Footnotes and Endnotes

### Footnote

```
This is a footnote[^footy].
```

Output: This is a footnote[^footy].

[^footy]: Footnotes can be notes, sources, etc.

### Endnote

```
This is an endnote[^^endy].
```

Output: This is a endnote[^^endy].

[^^endy]: Endnotes can be notes, sources, etc.

## Crosslinks and ids

There are two parts to making a crosslink.

1. Define an id.
2. Reference that id with a crosslink.


### Defining an id

There are two ways to define an id:

1. Using an id attribute `{id: some-id}` in an attribute list which can contain other attributes.
2. Using a shorter "syntactic sugar" approach when the id is by itself: `{#some-id}`

The shorter approach is preferred. 

Examples:

~~~
{#some-id}
This is a paragraph with the id of `some-id`.
~~~

~~~
The [quick sly fox]{#quick_sly} jumped over the lazy dogs.
~~~

### Referencing an id With A Crosslink

Regardless of how you defined the id, you then link to it to create a crosslink. To do this, you use the `#` character and the id in a link:

~~~
[link text](#some-id)
~~~

# Metadata


## Attributes

An attribute list is one or more key-value, comma-separated pairs:

`{key_one: value1, key_two: value_two, key_three: "value three!", key_four: true, key_five: 0, key_six: 3.14}`

An attribute list can be inserted in one of three ways:

1. Immediately above a block element (e.g. heading, figure, etc), with **one newline** separating it from the block element.
2. Immediately after a span element (e.g. a word, italicized phrase, etc), with **no spaces** separating it from the span element.
3. On a line by itself, with one blank line above and below it. In this format, the attribute list contains [directives](#directives).


## Index Attributes

Index entries can either be attached to block or span elements using the same attribute list syntax. 

These are the various formats of an index entry:

~~~
{i: hello}
{i: "hello"}
{i: "Armstrong, Peter"}
{i: "Yahoo\!"}
{i: "*hello*"}
{i: "**hello**"}
{i: "hello!Peter"}
{i: "hello!*Peter*"}
{i: "hello!**Peter**"}
{i: "Peter|see{i:'hello'}"}
{i: "Jen|seealso{i:'Jenny'}"}
~~~

Here's what they do:

`{i: hello}`
: Adds an index entry for `hello`. If an index entry has no punctuation or formatting then it does not need quotes.

`{i: "hello"}`
: Adds an index entry for `hello`. Quotes are always fine to use, even when not required.

`{i: "Armstrong, Peter"}`
: Adds an index entry for `Armstrong, Peter`. The quotes are always omitted. Their function is to allow things like exclamation marks and other punctuation to be added without fear, in case you don't feel like learning which punctuation is safe.

`{i: "Yahoo\!"}`
: Adds an index entry for `Yahoo!`. Note that the exclamation mark must be backslash-escaped because `!` is a delimiter otherwise. The `|`, `{`, `}` and `\` characters also must be backslash-escaped.

`{i: "*hello*"}`
: Adds an index entry for `hello`, with `hello` in italics.

`{i: "**hello**"}`
: Adds an index entry for `hello`, with `hello` in bold.

`{i: "hello!Peter"}`
: Adds an index entry for `Peter` which is a sub-entry of `hello`.

`{i: "hello!*Peter*"}`
: Adds an index entry for `Peter` (with *Peter* in emphasis) which is a sub-entry of `hello`. Note that this cannot be combined with a see or seealso (the | syntax).

`{i: "hello!**Peter**"}`
: Adds an index entry for `Peter` (with **Peter** in strong emphasis) which is a sub-entry of `hello`. Note that this cannot be combined with a see or seealso (the | syntax).

`{i: "Peter|see{i:'hello'}"}`
: Adds an index entry for `Peter`, which references the index entry `hello` with the equivalent of "see" in the language of the book. Note that this cannot be combined with a sub-entry (the ! syntax).

`{i: "Jen|seealso{i:'Jenny'}"}`
: Adds an index entry for `Jen`, which references the index entry `Jenny` with the equivalent of "see also" in the language of the book. Note that this cannot be combined with a sub-entry (the ! syntax).

Index entries are case sensitive. For example, `{i: "mark"}` and `{i: "Mark"}` are distinct entries. (The first is for a result or a smudge, the second is a person's name.)

To attach an index entry to the start of a block, put it on its own line above a block:

~~~
{i: "hello"}
I just came to say hello, hello, hello, hello
~~~

To attach an index entry to a word, just add the index entry after the word:

~~~
I just came to say hello{i: "hello"}, hello, hello, hello
~~~

## Directives

The syntax for directives is simple: they are just contained in an attribute list. The only difference is that the attribute list is inserted an a line by itself, with one blank line above and below it.


### Section Directives

You add a book `section` directive like this:

`{section: mainmatter}`

The following values of the `section` directive can occur in front matter:

* `half-title`
* `series-title`
* `title-page`
* `copyright`
* `dedication`
* `epigraph`
* `toc`
* `figures`
* `tables`
* `foreword`
* `preface`
* `acknowledgments` (note that this value can also typically occur after the `{section: mainmatter}` book section directive)
* `introduction`
* `abbr` (yes, it's called `abbr` and not `abbreviations`, and note that this can also typically occur after the `{section: mainmatter}` book section directive)
* `chronology` (note that this can also typically occur after the `{section: mainmatter}` book section directive)

The `{section: mainmatter}` value indicates that the front matter is over. It is the start of the first page of the text.

The following values of the `section` directive can occur in back matter:

* `appendices`
* `notes`
* `glossary`
* `bibliography` (note that a Markua processor may wish to format the text inside this section appropriately)
* `contributors`
* `illustration-credits`
* `index`

## Settings Metadata

Settings are newline-separated key-value pairs, typically specified at the beginning of the first file. 

Example: 

~~~
{
title: Markua Specification
authors: Peter Armstrong
contributors: Scott Patten, Braden Simpson and Jordan Ell
copyright: Peter Armstrong
}
~~~

## Escaping Special Characters

Opening **curly braces** need to be escaped with a backslash:

~~~
\{this is an actual curly brace}
{this is an attribute list}
~~~

Output:
\{this is an actual curly brace}
{this is an attribute list}

Backticks are also special characters. To escape a backtick, you need to type two backticks. 

~~~
This is an ``actual`` backtick.
This backtick is interpreted as an `inline span` resource.
~~~

OUtput:
This is an ``actual`` backtick.
This backtick is interpreted as an `inline span` resource.