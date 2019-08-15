# Basic Syntax {#basic-syntax}

Nearly all Markdown applications support the basic syntax outlined in John Gruber's original design document. There are minor variations and discrepancies between Markdown processors — those are noted inline wherever possible.

T> Using Markdown doesn't mean that you can't also use HTML. You can add HTML tags to any Markdown file. This is helpful if you prefer certain HTML tags to Markdown syntax. For example, some people find that it's easier to use HTML tags for images.

## Headings {#headings}

To create a heading, add number signs (`#`) in front of a word or phrase. The number of number signs you use should correspond to the heading level. For example, to create a heading level three (`<h3>`), use three number signs (e.g., `### My Header`).

| Markdown                       | HTML                       |
|--------------------------------|----------------------------|
| `# Heading level 1`            | `<h1>Heading level 1</h1>` |
| `## Heading level 2`           | `<h2>Heading level 2</h2>` |
| `### Heading level 3`          | `<h3>Heading level 3</h3>` |
| `#### Heading level 4`         | `<h4>Heading level 4</h4>` |
| `##### Heading level 5`        | `<h5>Heading level 5</h5>` |
| `###### Heading level 6`       | `<h6>Heading level 6</h6>` |

### Alternate Syntax

Alternatively, on the line below the text, add any number of `==` characters for heading level 1 or `--` characters for heading level 2.

| Markdown                       | HTML                                   |
|--------------------------------|----------------------------------------|
| `Heading level 1`              | `<h1>Heading level 1</h1>`             |
| `===============`              |                                        |
|--------------------------------|----------------------------------------|
| `Heading level 2`              | `<h2>Heading level 2</h2>`             |
| `---------------`              |                                        |


## Paragraphs

To create paragraphs, use a blank line to separate one or more lines of text. You should not indent paragraphs with spaces or tabs.

{title="Markdown"}
~~~~~~~
I really like using Markdown.

I think I'll use it from now on.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<p>I really like using Markdown.</p>

<p>I think I'll use it from now on.</p>
~~~~~~~

The rendered output looks like this:

I really like using Markdown.

I think I'll use it from now on.

## Line Breaks

To create a line break (`<br>`), end a line with two or more spaces, and then type return.

{title="Markdown"}
~~~~~~~
This is the first line.  
And this is the second line.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<p>This is the first line.<br />
And this is the second line.</p>
~~~~~~~

The rendered output looks like this:

This is the first line.  
And this is the second line.

## Emphasis {#emphasis}

You can add emphasis by making text bold or italic.

### Bold {#bold}

To bold text, add two asterisks or underscores before and after a word or phrase. To bold the middle of a word for emphasis, add two asterisks without spaces around the letters.

{title="Markdown"}
~~~~~~~
I love **bold text**.

I love __bold text__.

Love**is**bold
~~~~~~~

The HTML output of the first two examples is the same.

{title="HTML", lang=html}
~~~~~~~
I love <strong>bold text</strong>.

Love<strong>is</strong>bold
~~~~~~~

The rendered output looks like this:

I love **bold text**.

Love**is**bold

### Italic {#italic}

To italicize text, add one asterisk or underscore before and after a word or phrase. To italicize the middle of a word for emphasis, add one asterisk without spaces around the letters.

{title="Markdown"}
~~~~~~~
The *cat's meow*.

The _cat's meow_.

A*cat*meow
~~~~~~~

The HTML output of the first two examples is the same.

{title="HTML", lang=html}
~~~~~~~
The <em>cat's meow</em>.

A<em>cat</em>meow
~~~~~~~

The rendered output looks like this:

The *cat's meow*.

A*cat*meow

### Bold and Italic

To emphasize text with bold and italics at the same time, add three asterisks or underscores before and after a word or phrase.

{title="Markdown"}
~~~~~~~
***Important*** text.

___Important___ text.

__*Important*__ text.

**_Important_** text.
~~~~~~~

The HTML output of all four examples is the same.

{title="HTML", lang=html}
~~~~~~~
<strong><em>Important</em></strong> text.
~~~~~~~

The rendered output looks like this:

***Important*** text.

## Blockquotes {#blockquotes}

To create a blockquote, add a `>` in front of a paragraph.

{title="Markdown"}
~~~~~~~
> Dorothy followed her through many rooms.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<blockquote>
  <p>Dorothy followed her through many rooms.</p>
</blockquote>
~~~~~~~

The rendered output looks like this:

> Dorothy followed her through many rooms.

### Blockquotes with Multiple Paragraphs

Blockquotes can contain multiple paragraphs. Add a `>` on the blank lines between the paragraphs.

{title="Markdown"}
~~~~~~~
> This the first paragraph.
>
> And this is the second paragraph.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<blockquote>
  <p>This the first paragraph.</p>
  <p>And this is the second paragraph.</p>
</blockquote>
~~~~~~~

The rendered output looks like this:

> This the first paragraph.
>
> And this is the second paragraph.

### Nested Blockquotes

Blockquotes can be nested. Add a `>>` in front of the paragraph you want to nest.

{title="Markdown"}
~~~~~~~
> This the first paragraph.
>
>> And this is the nested paragraph.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<blockquote>
  <p>This the first paragraph.</p>
  <blockquote>
    <p>And this is the nested paragraph.</p>
  </blockquote>
</blockquote>
~~~~~~~

The rendered output looks like this:

> This the first paragraph.
>
>> And this is the nested paragraph.

### Blockquotes with Other Elements

Blockquotes can contain other Markdown formatted elements. Not all elements can be used — you’ll need to experiment to see which ones work.

{title="Markdown"}
~~~~~~~
> ##### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going **well**.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<blockquote>
  <h5>The quarterly results look great!</h5>
  <ul>
    <li>Revenue was off the chart.</li>
    <li>Profits were higher than ever.</li>
  </ul>
  <p><em>Everything</em> is going <strong>well</strong>.</p>
</blockquote>
~~~~~~~

The rendered output looks like this:

> ##### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going **well**.

## Lists

You can organize items into ordered and unordered lists.

### Ordered Lists {#ordered-lists}

To create an ordered list, add line items with numbers followed by periods. The numbers don’t have to be in numerical order, but the list should start with the number one.

{title="Markdown"}
~~~~~~~
1. First item
2. Second item
3. Third item
4. Fourth item

1. First item
1. Second item
1. Third item
1. Fourth item

1. First item
8. Second item
3. Third item
5. Fourth item
~~~~~~~

The HTML output of all three example lists is the same.

{title="HTML", lang=html}
~~~~~~~
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item</li>
</ol>
~~~~~~~

The rendered output looks like this:

1. First item
2. Second item
3. Third item
4. Fourth item

#### Nesting List Items

To nest line items in an ordered list, indent the items four spaces or one tab.

{title="Markdown"}
~~~~~~~
1. First item
2. Second item
3. Third item
    1. Indented item
    2. Indented item
4. Fourth item
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item
    <ol>
      <li>Indented item</li>
      <li>Indented item</li>
    </ol>
  </li>
  <li>Fourth item</li>
</ol>
~~~~~~~

The rendered output looks like this:

1. First item
2. Second item
3. Third item
    1. Indented item
    2. Indented item
4. Fourth item

### Unordered Lists {#unordered-lists}

To create an unordered list, add dashes (`-`), asterisks (`*`), or plus signs (`+`) in front of line items.

{title="Markdown"}
~~~~~~~
- First item
- Second item
- Third item
- Fourth item

* First item
* Second item
* Third item
* Fourth item

+ First item
* Second item
- Third item
+ Fourth item
~~~~~~~

The HTML output of all three example lists is the same.

{title="HTML", lang=html}
~~~~~~~
<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item </li>
</ul>
~~~~~~~

The rendered output looks like this:

- First item
- Second item
- Third item
- Fourth item

#### Nesting List Items

To nest line items in an unordered list, indent the items four spaces or one tab.

{title="Markdown"}
~~~~~~~
- First item
- Second item
- Third item
    - Indented item
    - Indented item
- Fourth item
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item
    <ul>
      <li>Indented item</li>
      <li>Indented item</li>
    </ul>
  </li>
  <li>Fourth item</li>
</ul>
~~~~~~~

The rendered output looks like this:

- First item
- Second item
- Third item
    - Indented item
    - Indented item
- Fourth item

### Adding Elements in Lists

To add another element in a list while preserving the continuity of the list, indent the element four spaces or one tab, as shown in the following examples.

#### Paragraphs

{title="Markdown"}
~~~~~~~
*   This is the first list item.
*   Here's the second list item.

    I need to add another paragraph below the second list item.

*   And here's the third list item.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<ul>
  <li><p>This is the first list item.</p></li>
  <li><p>Here's the second list item.</p>
    <p>I need to add another paragraph below the second list item.</p>
  </li>
  <li><p>And here's the third list item.</p></li>
</ul>
~~~~~~~

The rendered output looks like this:

*   This is the first list item.
*   Here's the second list item.

    I need to add another paragraph below the second list item.

*   And here's the third list item.

#### Blockquotes

{title="Markdown"}
~~~~~~~
*   This is the first list item.
*   Here's the second list item.

    > A blockquote would look great here.

*   And here's the third list item.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<ul>
  <li><p>This is the first list item.</p></li>
  <li><p>Here's the second list item.</p>
    <blockquote>
      <p>A blockquote would look great here.</p>
    </blockquote>
  </li>
  <li><p>And here's the third list item.</p>
  </li>
</ul>
~~~~~~~

The rendered output looks like this:

*   This is the first list item.
*   Here's the second list item.

    > A blockquote would look great here.

*   And here's the third list item.

#### Code Blocks

[Code blocks](#code-blocks) are normally indented four spaces or one tab. When they’re in a list, indent them eight spaces or two tabs.

{title="Markdown"}
~~~~~~~
1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3.  Update the title to match the name of your website.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<ol>
  <li><p>Open the file.</p></li>
  <li><p>Find the following code block on line 21:</p>
    <pre><code>&lt;html&gt;
      &lt;head&gt;
        &lt;title&gt;Test&lt;/title&gt;
      &lt;/head&gt;
    </code></pre>
  </li>
  <li><p>Update the title to match the name of your website.</p></li>
</ol>
~~~~~~~

The rendered output looks like this:

1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3.  Update the title to match the name of your website.

#### Images

{title="Markdown"}
~~~~~~~
1.  Open the file containing Tux, the Linux mascot.
2.  Marvel at its beauty.

    ![Tux](images/tux.png)

3.  Close the file.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<ol>
  <li><p>Open the file containing Tux, the Linux mascot.</p></li>
  <li>
    <p>Marvel at its beauty.</p>
    <p><img src="images/tux.png" alt="Tux" /></p>
  </li>
  <li><p>Close the file.</p></li>
</ol>
~~~~~~~

The rendered output looks like this:

1.  Open the file containing Tux, the Linux mascot.
2.  Marvel at its beauty.

    ![Tux](images/tux.png)

3.  Close the file.

## Code {#code}

To denote a word or phrase as code, enclose it in tick marks (`` ` ``).

{title="Markdown"}
~~~~~~~
At the command prompt, type `nano`.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
At the command prompt, type <code>nano</code>.
~~~~~~~

The rendered output looks like this:

At the command prompt, type `nano`.

### Escaping Tick Marks {#escaping-tick-marks}

If the word or phrase you want to denote as code includes one or more tick marks, you can escape it by enclosing the word or phrase in double tick marks (`` `` ``).

{title="Markdown"}
~~~~~~~
``Use `code` in your Markdown file.``
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<code>Use `code` in your Markdown file.</code>
~~~~~~~

The rendered output looks like this:

``Use `code` in your Markdown file.``

### Code Blocks {#code-blocks}

To create code blocks, indent every line of the block by at least four spaces or one tab.

{title="Markdown"}
~~~~~~~
    <html>
      <head>
      </head>
    </html>
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<pre>
  <code>
    &lt;html&gt;
      &lt;head&gt;
      &lt;/head&gt;
    &lt;/html&gt;
  </code>
</pre>
~~~~~~~

The rendered output looks like this:

    <html>
      <head>
      </head>
    </html>

I> To create code blocks without indenting lines, use [fenced code blocks](#fenced-code-blocks).

## Horizontal Rules {#horizontal-rules}

To create a horizontal rule, use three or more asterisks (`***`), dashes (`---`), or underscores (`___`) on a line by themselves.

{title="Markdown"}
~~~~~~~
***

---

_________________
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<hr />

<hr />

<hr />
~~~~~~~

The rendered output of all three looks identical:

***

## Links {#links}

To create a link, enclose the link text in brackets (e.g., `[Duck Duck Go]`) and then follow it immediately with the URL in parentheses (e.g., `(https://duckduckgo.com)`).

{title="Markdown"}
~~~~~~~
Use [Duck Duck Go](https://duckduckgo.com).
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<p>Use <a href="https://duckduckgo.com">Duck Duck Go</a>.</p>
~~~~~~~

The rendered output looks like this:

Use [Duck Duck Go](https://duckduckgo.com).

### Adding Titles

You can optionally add a title for a link. This will appear as a tooltip when the user hovers over the link. To add a title, enclose it in parentheses after the URL.

{title="Markdown"}
~~~~~~~
Use [Duck Duck Go](https://duckduckgo.com "My search engine!").
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<p>Use <a href="https://duckduckgo.com" title="My search engine!">Duck Duck Go</a>.</p>
~~~~~~~

The rendered output looks like this:

Use [Duck Duck Go](https://duckduckgo.com "My search engine!").

### URLs and Email Addresses

To quickly turn a URL or email address into a link, enclose it in angle brackets.

{title="Markdown"}
~~~~~~~
<https://eff.org>
<fake@example.com>
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<a href="https://eff.org">https://eff.org</a>
<a href="mailto:fake@example.com">fake@example.com</a>
~~~~~~~

The rendered output looks like this:

<https://eff.org>  
<fake@example.com>

### Formatting Links

To [emphasize](#emphasis) links, add asterisks before and after the brackets and parentheses.

{title="Markdown"}
~~~~~~~
I love supporting **[EFF](https://eff.org)**.
This is the *[EFF](https://eff.org)*.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<p>I love supporting <strong><a href="https://eff.org">EFF</a></strong>.
This is the <em><a href="https://eff.org">EFF</a></em>.</p>
~~~~~~~

The rendered output looks like this:

I love supporting **[EFF](https://eff.org)**.  
This is the *[EFF](https://eff.org)*.

### Reference-style Links

Reference-style links are a special kind of link that make URLs easier to display and read in Markdown. Reference-style links are constructed in two parts: the part you keep inline with your text and the part you store somewhere else in the file to keep the text easy to read.

#### Formatting the First Part of the Link

The first part of a reference-style link is formatted with two sets of brackets. The first set of brackets surrounds the text that should appear linked. The second set of brackets displays a label used to point to the link you’re storing elsewhere in your document.

Although not required, you can include a space between the first and second set of brackets. Also, the label in the second set of brackets is not case sensitive and can include letters, numbers, spaces, or punctuation.

This means the following example formats are all roughly equivalent for the first part of the link:

- `[hobbit-hole][1]`
- `[hobbit-hole] [1]`
- `[hobbit-hole][a]`
- `[hobbit-hole][A]`

#### Formatting the Second Part of the Link

The second part of a reference-style link is formatted with the following attributes:

1. The label, in brackets, followed immediately by a colon and at least one space (e.g., `[label]:` ).
2. The URL for the link, which you can optionally enclose in angle brackets.
3. The optional title for the link, which you can enclose in double quotes, single quotes, or parentheses.

This means the following example formats are all roughly equivalent for the second part of the link:

- `[hobbit-hole]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle`
- `[hobbit-hole]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"`
- `[hobbit-hole]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'`
- `[hobbit-hole]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)`
- `[hobbit-hole]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"`
- `[hobbit-hole]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'`
- `[hobbit-hole]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles)`

You can place this second part of the link anywhere in your Markdown document. Some people place them immediately after the paragraph in which they appear while other people place them at the end of the document (like endnotes or footnotes).

#### An Example Putting the Parts Together

Say you add a URL as a [standard URL link](#links) to a paragraph and it looks like this in Markdown:

{title="Markdown"}
~~~~~~~
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to eat: it was a [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"), and that means comfort.
~~~~~~~

{title="Markdown"}
~~~~~~~
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to eat: it was a [hobbit-hole][1], and that means comfort.

[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
~~~~~~~

In both instances above, the HTML for the link would be identical:

{title="HTML", lang=html}
~~~~~~~
<a href="https://en.wikipedia.org/wiki/Hobbit#Lifestyle" title="Hobbit lifestyles">hobbit-hole</a>
~~~~~~~

The output is also identical:

In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to eat: it was a [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle), and that means comfort.

## Images {#images}

To add an image, add an exclamation mark (`!`), followed by alt text in brackets, and the path or URL to the image asset in parentheses. You can optionally add a title after the URL in the parentheses.

{title="Markdown"}
~~~~~~~
![Philadelphia's Magic Gardens. This place was so cool!](images/philly-magic-garden.png "Philadelphia's Magic Gardens")
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<img src="images/philly-magic-garden.png" alt="Philadelphia's Magic Gardens. This place was so cool!" title="Philadelphia's Magic Gardens" />
~~~~~~~

The rendered output looks like this:

![Philadelphia's Magic Gardens. This place was so cool!](images/philly-magic-garden.png "Philadelphia's Magic Gardens")

## Escaping Characters

To display a literal character that would otherwise be used to format text in a Markdown document, add a backslash (`\`) in front of the character.

{title="Markdown"}
~~~~~~~
\* Without the backslash, this would be a bullet in an unordered list.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<p>* Without the backslash, this would be a bullet in an unordered list.</p>
~~~~~~~

The rendered output looks like this:

\* Without the backslash, this would be a bullet in an unordered list.

### Characters You Can Escape

You can use a backslash to escape the following characters.

| Character         | Name                  |
|-------------------|-----------------------|
| `\`               | backslash             |
| `` ` ``           | tick mark (see also [escaping tick marks in code](#escaping-tick-marks)) |
| `*`               | asterisk              |
| `_`               | underscore            |
| `{}`              | curly braces          |
| `[]`              | brackets              |
| `()`              | parentheses           |
| `#`               | pound sign            |
| `+`               | plus sign             |
| `-`               | minus sign (hyphen)   |
| `.`               | dot                   |
| `!`               | exclamation mark      |
| `|`               | pipe (see also [escaping pipe in tables](#escaping-pipe-characters-in-tables)) |
