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

## Summary

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


# TODO

More to come

# Writing Guidelines #

# Toolchain #

# TODO

Automation
* TextExpander

Writing
* Scrivener
* Gingko App
* TextMate

Idea Formation
* MindMeister
* Evernote
* Index Carts

Bibliography
* Zotero

Publishing
* WordPress (plugins?)
* LeanPub
* GitBook

Version Control, Collaboration, Change Tracking
* Git
* GitHub

## TextExpander