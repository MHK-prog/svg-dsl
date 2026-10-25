# ⚡ svg-dsl

> **A minimal, zero-dependency text DSL to sketch SVGs with automatic fillets, polar points, and arcs in real-time.**

[🚀 **Try Live Demo**](https://YOUR_USERNAME.github.io/svg-dsl/)

---

## ✨ Features

- **Zero Dependencies**: Pure HTML/CSS and Vanilla JS in a single self-contained file.
- **Auto-Fillet (`r10`)**: Automatic corner rounding using quadratic Bézier curves.
- **Polar & Relative Coordinates**: Define points relative to others (`B = A(30, -20)`) or by angle/distance (`C = B @ (40, 90)`).
- **Arcs & Curves**: Clean arc syntax (`A ~30~ B`) with bidirectional curvature.
- **Interactive Canvas**: Smooth pinch-to-zoom and pan on both mobile and desktop.
- **One-Click Export**: Copy the raw SVG code instantly.

---

## 📖 Quick Syntax

### 1. Points
```dsl
A = (20, 20)           # Absolute (x, y)
B = A(80, 0)           # Relative to A
C = B @ (50, 45)       # Polar: Distance @ Angle
```

### 2. Rounded Shapes (Fillet)
```dsl
A -- B -- C -- A : r10 stroke(#38bdf8) fill(none) width(2)
```

### 3. Arcs & Circles
```dsl
P1 ~40~ P2 : stroke(#f43f5e)
circle(A, 15) : stroke(#22c55e) fill(none)
```

---

## 🛠️ Local Development

No `npm install`, no build step. Just clone and open `index.html`:

```bash
git clone https://github.com/YOUR_USERNAME/svg-dsl.git
cd svg-dsl
open index.html
```

---

## 🤝 Contributing

Issues, feature suggestions, and PRs are welcome! Feel free to open an issue if you have ideas for new syntax or modifiers.

License: MIT
