
---

# Markdown Quick Reference

Below is a single Markdown document that demonstrates many common Markdown features. You can copy this into a file named `Markdown.md`. Feel free to add or remove sections based on your needs!

This document highlights the most common Markdown syntax and features. Simply copy and paste this into a `.md` file to have a quick reference.

## 1. Headings

Use `#` through `######` to create headings of different levels.

```markdown
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```



---

## 2. Text Formatting

### 2.1 Emphasis

- *Italic* (using asterisks)  
  ```markdown
  *Italic*
  ```
- _Italic_ (using underscores)  
  ```markdown
  _Italic_
  ```

- **Bold** (using double asterisks)  
  ```markdown
  **Bold**
  ```
- __Bold__ (using double underscores)  
  ```markdown
  __Bold__
  ```

- ***Bold and Italic***  
  ```markdown
  ***Bold and Italic***
  ```
- ___Bold and Italic___  
  ```markdown
  ___Bold and Italic___
  ```

### 2.2 Strikethrough

- ~~Strikethrough~~  
  ```markdown
  ~~Strikethrough~~
  ```

---

## 3. Paragraphs and Line Breaks

Simply write your text in separate lines for paragraphs:

```markdown
This is the first paragraph.

This is the second paragraph.
```

To force a line break, end a line with two or more spaces:

```markdown
This line ends with two spaces.  
So this text starts on a new line.
```

---

## 4. Blockquotes

Use `>` to create blockquotes. They can be nested by using multiple `>` characters.

```markdown
> This is a blockquote.

> > Nested blockquote.
```

> This is a blockquote.

> > Nested blockquote.

---

## 5. Lists

### 5.1 Unordered Lists

Use `-`, `+`, or `*` followed by a space to create unordered lists.

```markdown
- Item 1
- Item 2
  - Nested Item 2.1
  - Nested Item 2.2
- Item 3
```

- Item 1
- Item 2
  - Nested Item 2.1
  - Nested Item 2.2
- Item 3

### 5.2 Ordered Lists

Use numbers followed by a period (`1.`, `2.`, `3.`) to create ordered lists.

```markdown
1. First item
2. Second item
3. Third item
   1. Sub item
   2. Sub item
```

1. First item
2. Second item
3. Third item
   1. Sub item
   2. Sub item

---

## 6. Horizontal Rules

Use three or more asterisks (`***`), dashes (`---`), or underscores (`___`) on their own line.

```markdown
---
***
___
```

---

## 7. Links

### 7.1 Inline Links

```markdown
[This is a link](https://www.example.com)
```

[This is a link](https://www.example.com)

### 7.2 Reference Links

```markdown
[Reference-style link][example-ref]

[example-ref]: https://www.example.com "Optional Title"
```

[Reference-style link][example-ref]

[example-ref]: https://www.example.com "Optional Title"

---

## 8. Images

### 8.1 Inline Images

```markdown
![Markdown Logo](https://markdown-here.com/img/icon256.png)
```

![Markdown Logo](https://markdown-here.com/img/icon256.png)

### 8.2 Reference Style Images

```markdown
![Alt text][img-ref]

[img-ref]: https://markdown-here.com/img/icon256.png "Markdown Logo"
```

![Alt text][img-ref]

[img-ref]: https://markdown-here.com/img/icon256.png "Markdown Logo"

---

## 9. Code

### 9.1 Inline Code

Surround inline code with backticks:

```markdown
Use the `printf()` function to print to standard output.
```

Example: Use the `printf()` function to print to standard output.

### 9.2 Code Blocks

Use triple backticks (```) with an optional language identifier for syntax highlighting:

<details>
  <summary>Example in Markdown</summary>

  ```markdown
  ```python
  def hello_world():
      print("Hello, world!")
  ```
  ```
</details>

Which renders as:

```python
def hello_world():
    print("Hello, world!")
```

---

## 10. Tables

Use `|` to create tables. You can align columns using colons (`:`).

```markdown
| Left Align | Center Align | Right Align |
|:-----------|:------------:|------------:|
| Item A     |   Item B     |       Item C|
| Item D     |   Item E     |       Item F|
```

| Left Align | Center Align | Right Align |
|:-----------|:------------:|------------:|
| Item A     |   Item B     |       Item C|
| Item D     |   Item E     |       Item F|

---

## 11. Footnotes

Use `[^1]` syntax to add footnotes.

```markdown
Here is a sentence with a footnote.[^1]

[^1]: This is the footnote text.
```

Here is a sentence with a footnote.[^1]

[^1]: This is the footnote text.

---

## 12. Task Lists (GitHub Flavored Markdown)

You can create checklists using `- [ ]` or `- [x]`.

```markdown
- [x] Completed task
- [ ] Incomplete task
- [ ] Another task
```

- [x] Completed task  
- [ ] Incomplete task  
- [ ] Another task  

---

## 13. Emojis (GitHub / Some Editors)

You can use `:emoji_name:` to insert emojis (in some Markdown renderers like GitHub).

For example:

```markdown
:smiley: :thumbsup: :tada:
```

:smiley: :thumbsup: :tada:

---

## 14. HTML in Markdown

You can mix HTML for more complex layouts:

```markdown
<p style="color: blue;">This is a blue paragraph in HTML.</p>
```

<p style="color: blue;">This is a blue paragraph in HTML.</p>

---

## 15. Escaping Characters

Use a backslash to escape Markdown characters if needed:

```markdown
\*This text is not italicized.\*
```

\*This text is not italicized.\*

---

## 16. Collapsible Sections (GitHub Flavored Markdown)

<details>
  <summary>Click to expand!</summary>
  
  This is some hidden content!

</details>

```markdown
<details>
  <summary>Click to expand!</summary>
  
  This is some hidden content!

</details>
```

---

## That’s It!

This cheat sheet should cover the most commonly used Markdown syntax. Experiment, mix and match, and enjoy writing clean and visually appealing documentation!

Feel free to modify this document in any way you see fit. Happy writing!