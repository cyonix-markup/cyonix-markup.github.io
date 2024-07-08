# Getting started with Cyonix



Cyonix is meant for browser use and is not compatible within a Node.js environment.

Cyonix needs cSS from this style sheet: `https://cdn.jsdelivr.net/npm/cyonix@1.0.3/styles.min.css`

https://cdn.jsdelivr.net/npm/cyonix@1.0.3/cyonix.min.js

Cyonix is a markup language inspired by Markdown, designed for simplicity and flexibility.

## Functions

### parseCY(cyMarkup)

The `parseCY` function converts Cyonix markup into HTML.

#### Syntax Support

- **Headings**
  ```
  # Heading 1
  ## Heading 2
  ### Heading 3
  ```

- **Lists**
  ```
  * Item 1
  * Item 2
  1. Ordered Item 1
  2. Ordered Item 2
  ```

- **Checkboxes**
  ```
  * [ ] Unchecked item
  * [x] Checked item
  ```

- **Blockquotes**
  ```
  >> This is a blockquote
  ```

- **Links**
  ```
  {Link Text}(https://example.com)
  ```

- **Images**
  ```
  ![Alt Text]({image-url})
  ```

- **Code Blocks and Inline Code**
  ```
  ```
  Code block
  ```

  Inline `code`

- **Horizontal Rule**
  ```
  ---
  ```

- **Tables**
  ```
  | Header 1 | Header 2 |
  | -------- | -------- |
  | Cell 1   | Cell 2   |
  ```

- **Formatting**
  - **Bold**: `<<Bold Text>>`
  - **Italic**: `[[Italic Text]]`
  - **Strikethrough**: `~~Strikethrough Text~~`
  - **Keyboard Input**: `[Keyboard Input]`

### renderCY()

The `renderCY` function retrieves input from a textarea and renders the parsed HTML output.

#### Example Usage

```html
<textarea id="cy-input">
# Welcome to Cyonix

* [ ] Task 1
* [x] Task 2
</textarea>

<button onclick="renderCY()">Render Output</button>

<div id="html-output">
<!-- Rendered HTML output will appear here -->
</div>
```

## Example

Here's a simple example of Cyonix markup and its rendered HTML:

### Cyonix Markup

```markdown
# Welcome to Cyonix

* [ ] Task 1
* [x] Task 2
```

### Rendered HTML

```html
<h1>Welcome to Cyonix</h1>
<ul>
  <li><input type="checkbox"> Task 1</li>
  <li><input type="checkbox" checked> Task 2</li>
</ul>
```

This documentation provides a quick overview of Cyonix syntax and usage. For more detailed information, refer to the specific functions and examples provided.
