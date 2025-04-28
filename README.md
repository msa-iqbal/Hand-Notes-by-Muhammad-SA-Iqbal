# Markdown Cheat Sheet

## Table of Contents

1. [Headings](#headings)
2. [Bold](#bold)
3. [Italic](#italic)
4. [Bold & Italic](#bold--italic)
5. [Strikethrough](#strikethrough)
6. [Underline](#underline)
7. [Highlight](#highlight)
8. [Blockquote](#blockquote)
9. [Ordered List](#ordered-list)
10. [Unordered List](#unordered-list)
11. [Code](#code)
12. [Horizontal Rule](#horizontal-rule)
13. [Link](#link)
14. [Image](#image)
15. [Table](#table)
16. [Code Block](#code-block)
17. [Heading ID](#heading-id)
18. [Task List](#task-list)
19. [Emoji](#emoji)
20. [Mathematical Expressions](#mathematical-expressions)
21. [Dropdown](#dropdown)
22. [Footnotes](#footnotes)

## Headings

**Syntax:**

```markdown
# H1 - Heading 1

## H2 - Heading 2

### H3 - Heading 3

#### H4 - Heading 4

##### H5 - Heading 5

###### H6 - Heading 6
```

**Output:**

# H1 - Heading 1

## H2 - Heading 2

### H3 - Heading 3

#### H4 - Heading 4

##### H5 - Heading 5

###### H6 - Heading 6

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Bold

**Syntax:**

```markdown
**Bold Text**
```

**Output:**

**Bold Text**

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Italic

**Syntax:**

```markdown
_Italic Text_
```

**Output:**

_Italic Text_

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Bold & Italic

**Syntax:**

```markdown
_**Bold and Italic Text**_
```

**Output:**

_**Bold and Italic Text**_

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Strikethrough

It adds a horizontal line through the text.

**Syntax:**

```markdown
~~This text will be strikethrough~~
```

**Output:**

~~This text will be strikethrough~~

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Underline

Standard Markdown does not natively support underlining. However, you can simulate underlining by using HTML tags within your Markdown content. _(Not Recommended)_

**Example:**

```markdown
<u>This text will be underlined</u>
```

**Output:**

<u>This text will be underlined</u>

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Highlight

Markdown itself does not have built-in syntax for highlighting text. However, you can simulate highlighting in Markdown by using HTML tags, such as `<mark>`. _(Not Recommended)_

**Example:**

```markdown
This is <mark>highlighted</mark> text.
```

**Output:**

This is <mark>highlighted</mark> text.

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Blockquote

**Syntax (Basic):**

```markdown
> Blockquote
```

**Output:**

> Blockquote

**Syntax (Nested Blockquotes):**

```markdown
> This is a first-level blockquote.
>
> > This is a second-level (nested) blockquote.
> >
> > > This is a third-level (deeply nested) blockquote.
>
> Back to first-level blockquote.
```

**Output:**

> This is a first-level blockquote.
>
> > This is a second-level (nested) blockquote.
> >
> > > This is a third-level (deeply nested) blockquote.
>
> Back to first-level blockquote.

**Syntax (Blockquotes with Other Elements):**

````markdown
> To print in Python:
>
> ```javascript
> console.log("Hello, Always Smile!");
> ```
````

**Output:**

> ### To print in JavaScript
>
> ```javascript
> console.log("Hello, Always Smile!");
> ```

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Ordered List

**Syntax (Basic):**

```markdown
1. First item
1. Second item
1. Third item
```

**Output:**

1. First item
1. Second item
1. Third item

**Syntax (Nested Order List):**

```markdown
1. First item
   1. First nested item
   2. Second nested item
2. Second item
   1. First nested item
      1. Deeply nested item
3. Third item
```

**Output:**

1. First item
   1. First nested item
   2. Second nested item
2. Second item
   1. First nested item
      1. Deeply nested item
3. Third item

:bulb: Note: Numbers auto-fix, formatting (bold, italic, links) allowed, indent 4 spaces for sublists.

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Unordered List

**Syntax (Basic):**

```markdown
- Apple
- Banana
- Cherry
```

**Output:**

- Apple
- Banana
- Cherry

**Syntax (Nested Unordered List):**

```markdown
1. Frontend
   - HTML
   - CSS
     - Flexbox
     - Grid
   - JavaScript
1. Backend
   - Node.js
   - Express.js
```

**Output:**

1. Frontend
   - HTML
   - CSS
     - Flexbox
     - Grid
   - JavaScript
1. Backend
   - Node.js
   - Express.js

:bulb: Note: Numbers auto-fix, formatting (bold, italic, links) allowed, indent 4 spaces for sublists.

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Code

**Syntax:**

```
To declare a variable in JavaScript, use `let` or `const`.
```

**Output:**

To declare a variable in JavaScript, use `let` or `const`.

## Horizontal Rule

You can create a horizontal rule by using three or more dashes (---), asterisks (\*\*\*), or underscores (\_\_\_), each on its own line. Using `---` is preferred for a clean, professional appearance and aligns with GitHub-flavored Markdown standards; therefore, it is the recommended practice.

**Syntax:**

```markdown
---
```

**Output:**

---

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Link

**Syntax (Basic):**

```markdown
[My Fuel](https://www.flickr.com/photos/spnkhn/albums/)
```

**Output:**

[My Fuel](https://www.flickr.com/photos/spnkhn/albums/)

**Syntax (Adding Title):**

```markdown
[My Fuel](https://www.flickr.com/photos/spnkhn/albums/ "You're Welcome!")
```

**Output:**

[My Fuel](https://www.flickr.com/photos/spnkhn/albums/ "You're Welcome!")

**Syntax (Link with Inline Code):**

```markdown
[`My Fuel`](https://www.flickr.com/photos/spnkhn/albums/ "You're Welcome!")
```

**Output:**

[`My Fuel`](https://www.flickr.com/photos/spnkhn/albums/ "You're Welcome!")

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Image

**Syntax (Basic):**

```markdown
![Island](https://cdn.pixabay.com/photo/2022/05/31/07/01/island-7232868_1280.png)
```

**Output:**

![Island](https://cdn.pixabay.com/photo/2022/05/31/07/01/island-7232868_1280.png)

**Syntax (Image with Optional Title):**

```markdown
![Nature](./assets/images/view.jpg "My favourite place!")
```

**Output:**

![Nature](./assets/images/view.jpg "My favourite place!")

**Syntax (Image with Link):**

```markdown
[![Visit Google](./assets/images/signature.png)](https://www.flickr.com/photos/spnkhn/albums/)
```

**Output:**

[![My Fuel](./assets/images/signature.png)](https://www.flickr.com/photos/spnkhn/albums/)

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Table

**Syntax (Basic):**

```markdown
| Header 1 | Header 2 | Header 3 |
| -------- | -------- | -------- |
| Data 1   | Data 2   | Data 3   |
| Data 4   | Data 5   | Data 6   |
```

- `|` (pipe) - Separates columns
- `-` (dash) - Separates header from body

**Output:**

| Header 1 | Header 2 | Header 3 |
| -------- | -------- | -------- |
| Data 1   | Data 2   | Data 3   |
| Data 4   | Data 5   | Data 6   |

**Syntax (Column Alignment):**

```markdown
| Left Align | Center Align | Right Align |
| :--------- | :----------: | ----------: |
| Apple      |    Orange    |      Banana |
| Cherry     |    Mango     |      Carrot |
```

- `:---` - Left align
- `:---:` - Center align
- `---:` - Right align

**Output:**

| Left Align | Center Align | Right Align |
| :--------- | :----------: | ----------: |
| Apple      |    Orange    |      Banana |
| Cherry     |    Mango     |      Carrot |

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Code Block

**Syntax:**

````
``` <preferred_language>
    ---
       Your Code ...
           ---
    ---
```
````

:bulb: Note: For syntax highlighting, specify the language immediately after the first set of triple backticks. If no syntax highlighting is required, use `markdown` after the triple backticks _(recommended)_.

**Example:**

````
```javascript
const emojis = ["😀", "🎉", "🚀", "🌈", "🍕", "🐶", "🌟"];

function getRandomEmoji() {
  const randomIndex = Math.floor(Math.random() * emojis.length);
  return emojis[randomIndex];
}

// Example usage:
console.log("Your random emoji is:", getRandomEmoji());

```
````

**Output:**

```javascript
const emojis = ["😀", "🎉", "🚀", "🌈", "🍕", "🐶", "🌟"];

function getRandomEmoji() {
  const randomIndex = Math.floor(Math.random() * emojis.length);
  return emojis[randomIndex];
}

// Example usage:
console.log("Your random emoji is:", getRandomEmoji());
```

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Heading ID

If you want to link to another part of the same Markdown file (like a heading), you can do it like this:

Example if your heading is:

```markdown
## Introduction

Welcome to the project!

## Features & Benefits

This section describes features.

## What's New?

All new updates listed here.

### Subsection: Updates

Detailed minor updates.
```

You can link to it like:

```markdown
[Introduction](#introduction)
[Go to Features](#features--benefits)
[See What's New](#whats-new)
[Minor Updates](#subsection-updates)
```

It automatically gets an ID by:

- Converting all letters to lowercase,
- Replacing spaces with hyphens (-),
- Removing special characters (like punctuation).

- Example
  - `## Introduction` - Auto-Generated ID is - `#introduction`
  - `## Features & Benefits` - Auto-Generated ID is - `#features--benefits`
  - `## What's New?` - Auto-Generated ID is - `#whats-new`
  - `Subsection: Updates` - Auto-Generated ID is - `#subsection-updates`

**Output:**

## Introduction

Welcome to the project!

## Features & Benefits

This section describes features.

## What's New?

All new updates listed here.

### Subsection: Updates

Detailed minor updates.

[Introduction](#introduction)  
[Go to Features](#features--benefits)  
[See What's New](#whats-new)  
[Minor Updates](#subsection-updates)

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Task List

A task list lets you create checkboxes (☑ / ⏹) in Markdown.

Use:

- [ ] for unchecked tasks (a blank space inside the brackets).

- [x] for checked tasks (lowercase "x" inside the brackets).

**Syntax:**

```markdown
### :memo: To-Do List

- [ ] Learn Markdown basics
- [x] Set up GitHub repository
- [ ] Create README.md
- [x] Push first commit
```

**Output:**

### :memo: To-Do List

- [ ] Learn Markdown basics
- [x] Set up GitHub repository
- [ ] Create README.md
- [x] Push first commit

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Emoji

Emojis are small icons used to make Markdown documents more expressive and fun. They improve readability, highlight important parts, and add personality to your text!

**Example (Directly Copy-Paste Emoji):**

```markdown
I love coding! ☕
```

**Output:**

I love coding! ☕

**Example (GitHub-Style Emoji Shortcodes):**

```markdown
I love coding! :coffee:
```

**Output:**

I love coding! :coffee:

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Mathematical Expressions

In Markdown, you can display **mathematical expressions** using a combination of **inline HTML** and **MathJax** (or other rendering libraries like KaTeX). Markdown itself doesn’t directly support rendering mathematical formulas, but platforms like **GitHub**, **GitLab**, and others that use **MathJax** can interpret these formulas.

Here's a guide to writing **mathematical expressions** in Markdown:

### **Using LaTeX Syntax with MathJax/KaTeX**

Markdown doesn’t natively support **LaTeX** math rendering, but on platforms that support MathJax or KaTeX, you can write math expressions using **LaTeX syntax**.

#### Inline Math

Use **`$`** to wrap inline math expressions. For Example:

```latex
The formula for the area of a circle is $A = \pi r^2$.
```

Output:

The formula for the area of a circle is $A = \pi r^2$.

#### Display Math

Use **`$$`** for display math (equations centered on their own line). For Example:

```latex
$$
E = mc^2
$$
```

Output:

$$
E = mc^2
$$

### **Supported Operators and Functions**

You can use the following **LaTeX math operators** within Markdown:

- **Superscript and Subscript**: `x^2` for superscript, `x_1` for subscript
- **Fractions**: `\frac{a}{b}`
- **Sums and integrals**: `\sum`, `\int`
- **Square root**: `\sqrt{x}`
- **Greek letters**: `\alpha`, `\beta`, `\gamma`, etc.
- **Trigonometric functions**: `\sin`, `\cos`, `\tan`
- **Mathematical symbols**: `\pi`, `\infty`, `\geq`

Example: Complex Math Expression

```latex
$$
\int_{0}^{\infty} \frac{1}{x^2 + 1} dx = \frac{\pi}{2}
$$
```

Output:

$$
\int_{0}^{\infty} \frac{1}{x^2 + 1} dx = \frac{\pi}{2}
$$

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Dropdown

In pure Markdown, there is no built-in support for creating dropdowns (collapsible sections).
However, you can achieve dropdown-like (collapsible) behavior using HTML `<details>` and `<summary>` tags, which are supported on platforms like GitHub, GitLab, and others that allow HTML inside Markdown.

**Syntax (In HTML):**

```markdown
<details>
  <summary>Click to expand</summary>

Content inside the dropdown.

</details>
```

**Example:**

```markdown
<details>
  <summary>See More Details</summary>

Here is some hidden content that only appears when you click the dropdown!

- Point 1
- Point 2
- **Bold Content**
- [Link to somewhere](https://example.com)

</details>
```

**Output:**

<details>
  <summary>See More Details</summary>

Here is some hidden content that only appears when you click the dropdown!

- Point 1
- Point 2
- **Bold Content**
- [Link to somewhere](https://example.com)

</details>

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->

## Footnotes

To add a footnote in Markdown, you use the following format:

- Add a superscript reference number inside square brackets ([1]) where you want the footnote to appear.

- Below the text, provide the reference using the same number in square brackets, followed by a colon and the footnote content.

**Syntax(Basic):**

```markdown
This is a sentence with a footnote reference.[^1]

[^1]: This is the footnote content.
```

**Output:**

This is a sentence with a footnote reference.[^1]

[^1]: This is the footnote content.

**Syntax(Footnote with Links):**

```markdown
Learn more about Markdown at [Markdown Guide](https://www.markdownguide.org).
```

You can also include links inside footnotes. This is useful for providing references or citing sources.

**Output:**

Learn more about Markdown at [Markdown Guide](https://www.markdownguide.org)[^2].

[^2]: The source of Markdown documentation is [here](https://www.markdownguide.org/).

<!-- "Jump to Top" Start -->
<p align="right" style="font-size: 16px; font-weight: 600; margin-top: 24px;">
  <a href="#table-of-contents" style="text-decoration: none; color: #0366d6;">Jump to Top ⤴</a>
</p>
<!-- "Jump to Top" End -->
