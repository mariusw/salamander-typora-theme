---
title: Salamander Theme Preview
author: Marius
date: 2026-05-31
---

# The Art of Quiet Systems

Body text flows in warm beige. **Bold pushes to cream**, *italics stay italic*, and ~~strikethrough dims to brown~~. [Links are muted warm brown](#) and brighten on hover. Inline `code snippets` use the burnt orange accent. You can also ==highlight text== like this. Combined ***bold and italic*** also works.

---

## Headings

# H1 — Cream

## H2 — Light tan, underlined

### H3 — Gold

#### H4 — Gold, slightly smaller

##### H5 — Gold, smaller still

###### H6 — Muted uppercase

---

## Blockquotes

> A blockquote sits to the right of a warm amber border. The text is italic and slightly recessed — readable but clearly set apart from the body.

Nested blockquotes:

> Outer level quote.
>
> > Inner level — deeper nesting inherits the border style.
> >
> > > Third level, if you need it.

---

## Code

### JavaScript

```javascript
// Salamander theme — syntax colours
function greet(name) {
  const msg = "Hello, " + name
  return msg + "!"   // returns a greeting
}

const count = 42
```

### Python

```python
# Fibonacci sequence
def fibonacci(n: int) -> list[int]:
    seq = [0, 1]
    for i in range(2, n):
        seq.append(seq[i - 1] + seq[i - 2])
    return seq

result = fibonacci(10)
print(result)  # [0, 1, 1, 2, 3, 5, 8, 13, 21, 34]
```

### CSS

```css
:root {
  --bg:     #0E0A06;
  --text:   #CAB292;
  --accent: #D6831B;
}

body {
  background: var(--bg);
  color: var(--text);
  font-family: 'Plus Jakarta Sans', sans-serif;
}
```

---

## Lists

### Unordered

- First item with burnt orange marker
- Second item, body text colour
- Nested lists
  - Also inherit the orange marker
  - And the same text colour
    - Third level nesting

### Ordered

1. Step one
2. Step two
3. Step three
   1. Sub-step A
   2. Sub-step B

### Task list

- [x] Completed task
- [ ] Pending task
- [ ] Another pending task

---

## Tables

| Element   | Color       | Notes        |
|-----------|-------------|--------------|
| Body text | `#CAB292`   | Warm beige   |
| H1        | `#F5E6C8`   | Light cream  |
| Accent    | `#D6831B`   | Burnt orange |
| Links     | `#9A7A58`   | Muted brown  |
| Muted     | `#7D5E3D`   | Brown-grey   |

---

## Math

Inline math looks like $E = mc^2$ within a sentence. Block math gets its own styled area:

$$
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

$$
\sum_{n=1}^{\infty} \frac{1}{n^2} = \frac{\pi^2}{6}
$$

---

## Horizontal Rules

Three styles, all rendered identically:

---

***

___
