---
title: Narrative Text
authors:
  - name: Gwenaël Caër
exports:
  - format: pdf
    template: arxiv_two_column
---

## Basics

### Text formatting

**strong**, _emphasis_, `literal text`, \*escaped symbols\*

### Bullet points and numbered lists

- Lists can start with `-` or `*`
  * My other, nested
  * bullet point list!

1. My numbered list
2. has two points

### Task lists

- [x] Create a community around Jupyter Book
- [ ] Revolutionize technical communication

### Quotations

> We know what we are, but know not what we may be.
>
> -- Hamlet act 4, Scene 5

### Math equations

$ax^2 + bx + c = 0$

### Code blocks

```python
a, b = 10, 8
c = a + b

print("The sum of", a, "and", b, "is", c)
```

## Directives

### Images

```{image} https://www.odatis-ocean.fr/fileadmin/user_upload/Logo-Odatis_fullsize.png
```

### Admonitions

```{note}
```

```{tip}
```

```{warning}
```

### Dropdowns

:::{dropdown} Dropdown Title
:open:
Dropdown content
:::

### Cards

```{card} Card title
:header: The _Header_
:footer: Footer

Card content
```

### Grids

::::{grid} 1 1 2 3

:::{card}
:header: Text content ✏️
Structure books with text files and Jupyter Notebooks with minimal configuration.
:::

:::{card}
:header: MyST Markdown ✨
Write MyST Markdown to create enriched documents with publication-quality features.
:::

:::{card}
:header: Executable content 🔁
Execute notebook cells, store results, and insert outputs across pages.
:::
::::

### Diagrams

```{mermaid}
graph LR
    A[Start] --> B[Step 1: Collect Data]
    B --> C[Step 2: Process Data]
    C --> D{Success?}
    D -->|Yes| E[Finish]
    D -->|No| B
```