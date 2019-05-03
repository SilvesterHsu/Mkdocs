# Math Support
The PyMdown Extensions package can be installed with the following command:
```
pip install pymdown-extensions
```
The following list of extensions that are part of the PyMdown Extensions package are recommended to be used together with the Material theme:
```
markdown_extensions:
  - pymdownx.arithmatex
  - pymdownx.betterem:
      smart_enable: all
  - pymdownx.caret
  - pymdownx.critic
  - pymdownx.details
  - pymdownx.emoji:
      emoji_generator: !!python/name:pymdownx.emoji.to_svg
  - pymdownx.inlinehilite
  - pymdownx.magiclink
  - pymdownx.mark
  - pymdownx.smartsymbols
  - pymdownx.superfences
  - pymdownx.tasklist:
      custom_checkbox: true
  - pymdownx.tilde
```
## Arithmatex MathJax
Arithmatex integrates Material with MathJax which parses block-style and inline equations written in TeX markup and outputs them in mathematical notation. See this thread for a short introduction and quick reference on how to write equations in TeX syntax.

Besides activating the extension in the `mkdocs.yml`, the MathJax JavaScript runtime needs to be included. This must be done with additional JavaScript:
```
extra_javascript:
  - 'https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.0/MathJax.js?config=TeX-MML-AM_CHTML'
```

## Usage
### Inline Tex

**Example:**

```
This is an example: $x^2+y^2=1$
```

**Result:**

This is an example: $x^2+y^2=1$

### Blocks Tex

**Example:**

```
This is an example:
$$
\LaTeX
$$
```

**Result:**

This is an example:
$$
\LaTeX
$$
