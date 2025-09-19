---
title: Narrative Text
authors:
  - name: Gwenaël Caër
---

TO DO (Introduction)

## Basics

### Text formatting

- Bold: `**bold text**` → **bold text**  
- Italic: `*italic text*` → *italic text*  
- Strikethrough: `~~strikethrough~~` ~~strikethrough~~

### Bullet points list

* step 1
* step 2
* step 3

### Quotations

> This is a quote !

### Math equations

$ax^2 + bx + c = 0$

### Code blocks
```python
print("Hello World!")
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

### Dropwdowns

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
    A[Début] --> B[Étape 1]
    B --> C[Étape 2]
    C --> D[Fin]
```