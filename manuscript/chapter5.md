# Cheat Sheet {#cheat-sheet}

This cheat sheet provides a quick overview of all the Markdown syntax elements. It can't cover every edge case! If you need more information about any of these elements, refer back to the chapters on [basic](#basic-syntax) and [extended syntax](#extended-syntax).

## Basic Syntax

These are the elements outlined in John Gruber's original design document. All Markdown applications support these elements.

| Element           | Markdown Syntax                                      |
|-------------------|------------------------------------------------------|
| [Heading](#headings)  | `# H1`                                           |
|                   | `## H2`                                              |
|                   | `### H3`                                             |
|-------------------|------------------------------------------------------|
| [Bold](#bold)     | `**bold text**`                                      |
|-------------------|------------------------------------------------------|
| [Italic](#italic) | `*italicized text*`                                  |
|-------------------|------------------------------------------------------|
| [Blockquote](#blockquotes) |  `> blockquote`                             |
|-------------------|------------------------------------------------------|
| [Ordered List](#ordered-lists)   | `1. First item`                       |
|                   | `2. Second item`                                     |
|                   | `3. Third item`                                      |
|-------------------|------------------------------------------------------|
| [Unordered List](#unordered-lists) | `- First item`                      |
|                   | `- Second item`                                      |
|                   | `- Third item`                                       |
|-------------------|------------------------------------------------------|
| [Code](#code)     | `` `code` ``                                         |
|-------------------|------------------------------------------------------|
| [Horizontal Rule](#horizontal-rules)   |  `---`                          |
|-------------------|------------------------------------------------------|
| [Link](#links)    |  `[title](https://www.example.com)`                  |
|-------------------|------------------------------------------------------|
| [Image](#images)  |  `![alt text](image.jpg)`                            |


## Extended Syntax

These elements extend the basic syntax by adding additional features. Not all Markdown applications support these elements.

| Element           | Markdown Syntax                                      |
|-------------------|------------------------------------------------------|
| [Table](#tables)  | `| Syntax | Description |`                           |
|                   | `| ------ | ----------- |`                           |
|                   | `| Header | Title |`                                 |
|                   | `| Paragraph | Text |`                               |
|-------------------|------------------------------------------------------|
| [Fenced Code Block](#fenced-code-blocks) | ```` ``` ````                 |
|                   | `{`                                                  |
|                   |   `"firstName": "John",`                             |
|                   |   `"lastName": "Smith",`                             |
|                   |   `"age": 25`                                        |
|                   | `}`                                                  |
|                   | ```` ``` ````                                        |
|-------------------|------------------------------------------------------|
| [Footnote](#footnotes)  | `Here's a sentence with a footnote. [^1]`      |
|                   |                                                      |
|                   | `[^1]: This is the footnote.`                        |
|-------------------|------------------------------------------------------|
| [Heading ID](#heading-ids)  | `### My Great Heading {#custom-id}`        |
|-------------------|------------------------------------------------------|
| [Definition List](#definition-lists)  | `term`                           |
|                   | `: definition`                                       |
|-------------------|------------------------------------------------------|
| [Strikethrough](#strikethrough)  | `~~The world is flat.~~`              |
|-------------------|------------------------------------------------------|
| [Task List](#task-lists)  | `- [x] Write the press release`              |
|                   | `- [ ] Update the website`                           |
|                   | `- [ ] Contact the media`                            |

