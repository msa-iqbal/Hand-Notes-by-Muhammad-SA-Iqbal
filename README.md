# Markdown Cheat Sheet

1. [Headings](#headings)
2. [Bold](#bold)
3. [Italic](#italic)
4. [Blockquote](#blockquote)
5. [Ordered List](#ordered-list)
6. [Unordered List](#unordered-list)
7. [Code](#code)
8. [Horizontal Rule](#horizontal-rule)
9. [Link](#link)
10. [Image](#image)
11. [Table](#table)
12. [Code Block](#code-block)
13. [Footnotes](#footnotes)

## Headings

**Syntax:**

```plaintext
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

## Bold

**Syntax:**

```plaintext
**Bold Text**
```

**Output:**

**Bold Text**

## Italic

**Syntax:**

```plaintext
_Italic Text_
```

**Output:**

_Italic Text_

## Blockquote

**Syntax (Basic):**

```plaintext
> Blockquote
```

**Output:**

> Blockquote

**Syntax (Nested Blockquotes):**

```plaintext
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

````plaintext
> To print in Python:
>
> ```javascript
> print("Hello, Always Smile!")
> ```
````

**Output:**

> ### To print in JavaScript
>
> ```javascript
> print("Hello, Always Smile!");
> ```

## Ordered List

**Syntax (Basic):**

```plaintext
1. First item
1. Second item
2. Third item
```

**Output:**

1. First item
1. Second item
1. Third item

**Syntax (Nested Order List):**

```plaintext
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

💡 Note: Numbers auto-fix, formatting (bold, italic, links) allowed, indent 4 spaces for sublists.

## Unordered List

**Syntax (Basic):**

```plaintext
- Apple
- Banana
- Cherry
```

**Output:**

- Apple
- Banana
- Cherry

**Syntax (Nested Unordered List):**

```plaintext
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

💡 Note: Numbers auto-fix, formatting (bold, italic, links) allowed, indent 4 spaces for sublists.

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

```plaintext
---
```

**Output:**

---

## Link

**Syntax (Basic):**

```plaintext
[My Fuel](https://www.flickr.com/photos/spnkhn/albums/)
```

**Output:**

[My Fuel](https://www.flickr.com/photos/spnkhn/albums/)

**Syntax (Adding Title):**

```plaintext
[My Fuel](https://www.flickr.com/photos/spnkhn/albums/ "You're Welcome!")
```

**Output:**

[My Fuel](https://www.flickr.com/photos/spnkhn/albums/ "You're Welcome!")

**Syntax (Link with Inline Code):**

```plaintext
[`My Fuel`](https://www.flickr.com/photos/spnkhn/albums/ "You're Welcome!")
```

**Output:**

[`My Fuel`](https://www.flickr.com/photos/spnkhn/albums/ "You're Welcome!")

**❖❖❖ Internal Link:**

If you want to link to another part of the same Markdown file (like a heading), you can do it like this:

Example if your heading is:

```plaintext
## Installation Guide
```

You can link to it like:

```plaintext
[Go to Installation](#installation-guide)
```

**Output:**

[Go to Installation](#installation-guide)

## Image

**Syntax (Basic):**

```plaintext
![Island](https://cdn.pixabay.com/photo/2022/05/31/07/01/island-7232868_1280.png)
```

**Output:**

![Island](https://cdn.pixabay.com/photo/2022/05/31/07/01/island-7232868_1280.png)

**Syntax (Image with Optional Title):**

```plaintext
![Nature](./assets/images/view.jpg "My favourite place!")
```

**Output:**

![Nature](./assets/images/view.jpg "My favourite place!")

**Syntax (Image with Link):**

```plaintext
[![Visit Google](./assets/images/signature.png)](https://www.flickr.com/photos/spnkhn/albums/)
```

**Output:**

[![My Fuel](./assets/images/signature.png)](https://www.flickr.com/photos/spnkhn/albums/)

## Table

**Syntax (Basic):**

```plaintext
| Header 1 | Header 2 | Header 3 |
|----------|----------|----------|
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

```plaintext
| Left Align | Center Align | Right Align |
|:-----------|:------------:|------------:|
| Apple      |   Orange     |        Banana |
| Cherry     |   Mango      |        Carrot |
```

- `:---` - Left align
- `:---:` - Center align
- `---:` - Right align

**Output:**

| Left Align | Center Align | Right Align |
| :--------- | :----------: | ----------: |
| Apple      |    Orange    |      Banana |
| Cherry     |    Mango     |      Carrot |

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

💡 Note: For syntax highlighting, specify the language immediately after the first set of triple backticks. If no syntax highlighting is required, use `plaintext` after the triple backticks _(recommended)_.

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

## Footnotes

To add a footnote in Markdown, you use the following format:

- Add a superscript reference number inside square brackets ([1]) where you want the footnote to appear.

- Below the text, provide the reference using the same number in square brackets, followed by a colon and the footnote content.

**Syntax(Basic):**

```plaintext
This is a sentence with a footnote reference.[^1]

[^1]: This is the footnote content.
```

**Output:**

This is a sentence with a footnote reference.[^1]

[^1]: This is the footnote content.

**Syntax(Footnote with Links):**

```plaintext
Learn more about Markdown at [Markdown Guide](https://www.markdownguide.org).
```

You can also include links inside footnotes. This is useful for providing references or citing sources.

**Output:**

Learn more about Markdown at [Markdown Guide](https://www.markdownguide.org)[^1].

[^1]: The source of Markdown documentation is [here](https://www.markdownguide.org/).

