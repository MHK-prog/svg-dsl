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
