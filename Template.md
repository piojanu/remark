name: title
class: center, middle, title

# \\(\KaTeX{}\\) in remark
with code samples

---

.left-column[
 ## \\(\KaTeX{}\\)
### - Formulas
]

.right-column[
## Inline formulas:

1. This is an inline integral: \\(\int_a^bf(x)dx\\)
2. More \\(x={a \over b}\\) formulate.

## Display formula:

$$e^{i\pi} + 1 = 0$$
]

---

.left-column[
 ## \\(\KaTeX{}\\)
### - Formulas
### - Code
]

.right-column[
.pull-left[
## Inline:

```markdown
\\(\int_a^bf(x)dx\\)
\\(x={a \over b}\\)
```
]

.pull-right[
## Display:

```markdown
$$e^{i\pi} + 1 = 0$$
```
]

This code represents how to write LaTeX formulas. You can inline them (left) with other content or put them in their own block (right).

.footnote[.red[*] Example footnote :)]
]

---

# HTML sample

```xml
<!DOCTYPE html>
<html>
  <head>
    <style type="text/css">
      /* Slideshow styles */
    </style>
  </head>
  <body>
*    <textarea id="source">
      <!-- Slideshow Markdown -->
    &lt;/textarea&gt;
*    <script src="remark.js">
    </script>
    <script>
*      var slideshow = remark.create();
    </script>
  </body>
</html>
```
