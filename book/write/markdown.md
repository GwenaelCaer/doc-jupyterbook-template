---
title: Narrative Text
authors:
  - name: Gwenaël Caër
---

# Introduction

This document introduces the **Markdown** language and its **MyST** (Markedly Structured Text) extensions, used in particular in Jupyter Books and scientific documentation.  
The goal is to show, through examples, how to write structured text, add special blocks, and enrich your documents.

---

## Basics

### Text formatting

Markdown makes it easy to format text:

- `**text between two asterisks**` → **bold**  
- `_text between underscores_` → _italic_  
- `` `text surrounded by backticks` `` → `inline code`  
- The backslash `\` lets you escape a special character: for example, `\*` displays as \*.

---

### Bullet points and numbered lists

You can easily create lists:

- Bulleted lists are defined with `-` or `*`.  
- Numbered lists use `1.`, `2.`, etc.  
- Indentation allows you to nest sub-lists.

Example:  

- First point  
  * sub-point  
  * another sub-point  

1. First numbered item  
2. Second numbered item  

---

### Task lists

Markdown (and MyST) can also create **task lists**:

- `[x]` checks a box  
- `[ ]` leaves a box empty  

Example:  

- [x] Build a community around Jupyter Book  
- [ ] Revolutionize technical communication  

---

### Quotations

To insert a quotation, use `>` at the beginning of the lines:  

> We know what we are, but know not what we may be.  
>  
> -- Hamlet Act 4, Scene 5  

---

### Math equations

Math formulas can be integrated using LaTeX:  

```markdown
$ax^2 + bx + c = 0$
````

Result: \$ax^2 + bx + c = 0\$

---

### Code blocks

Code blocks are defined with three backticks followed by the language (here `python`):

```python
a, b = 10, 8
c = a + b
print("The sum of", a, "and", b, "is", c)
```

---

## Directives with MyST

Directives are an extension of Markdown, provided by MyST. They allow you to add rich elements such as images, notes, grids, or diagrams.

---

### Images

With the `{image}` directive, you can insert an external image:

```{image} https://www.odatis-ocean.fr/fileadmin/user_upload/Logo-Odatis_fullsize.png
```

---

### Admonitions

Admonitions are informational boxes.
You can use `{note}`, `{tip}`, or `{warning}` for different types of messages:

```{note}
This is a note.
```

```{tip}
Here is a tip.
```

```{warning}
Warning, this is an alert.
```

---

### Dropdowns

The `{dropdown}` directive creates collapsible content, useful for hiding secondary details:

```
:::{dropdown} Menu title
:open:
Menu content
:::
```

---

### Cards

The `{card}` directive allows you to structure content into cards with a header, content, and a footer:

```{card} Card title
:header: Header
:footer: Footer

Card content
```

---

### Grids

Going further, the `{grid}` directive allows you to arrange multiple cards or elements in columns. This is useful for creating structured layouts. Example:

```
::::{grid} 1 1 2 3

:::{card}
:header: Text ✏️
Structure your books with text files and notebooks.
:::

:::{card}
:header: MyST Markdown ✨
Use MyST to create enriched documents with advanced features.
:::

:::{card}
:header: Execution 🔁
Run code and automatically insert the results.
:::
::::
```

---

### Diagrams

Finally, MyST also makes it possible to integrate diagrams with Mermaid:

```{mermaid}
graph LR
    A[Start] --> B[Step 1: Collect Data]
    B --> C[Step 2: Process Data]
    C --> D{Success?}
    D -->|Yes| E[Finish]
    D -->|No| B
```

---

# Conclusion

Markdown provides a simple syntax for writing structured text.
With **MyST**, you gain access to advanced features that make documents interactive, rich, and suitable for scientific publishing.
