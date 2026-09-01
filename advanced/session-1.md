---
title: "Session 1 — Linear Algebra I"
layout: default
parent: Advanced track
nav_order: 1
---

# Session 1 — Linear Algebra I

Everything in linear algebra is built from two operations: **adding** vectors and
**scaling** them. This session goes from that starting point to the matrix as a
transformation of space, and along the way sets up the running example used for
the rest of the course — a small table of five participants measured on three
things (reaction time, accuracy, an anxiety score). A row is a participant, a
column is a measure, and both are vectors.

Nothing here is new mathematics for most of you. The aim is to make it *usable*.

**Length:** ~110 min, including four short practice breaks (7 min each).

## Topics covered

### Vectors, span, independence

- One object, three readings: an **arrow** (length and angle), a **point** (one row
  of a table), a **list** (how data actually arrives)
- Adding tip-to-tail, scaling along a line — and why one vector spans only a line
- **Linear combination**: the single operation everything else is a question about
- **Span** as a line, a plane, or a flat of higher dimension — always through the origin
- **Linear independence** via the vanishing combination, not "they look different"
- In $\mathbb{R}^n$, any $n+1$ vectors are dependent — the counting argument that
  *rank* will rest on next session

### The dot product and projection

- The two formulas: $\sum a_i b_i$ and $\lVert a\rVert\lVert b\rVert\cos\alpha$ —
  one computes, the other explains
- Norm, and what the **sign** of the dot product says about the angle
- **Projection**: the shadow and the residual — "explained plus unexplained"
- A coordinate in an orthonormal basis *is* a dot product
- **Cauchy–Schwarz** and cosine similarity; why the dot product itself is not bounded by 1
- A weighted score is a dot product — and a profile orthogonal to the scoring rule
  is not weakly seen, it is **invisible**

### Orthonormal bases and change of basis

- A basis as axes you *choose*; orthonormal means every coordinate is a projection
- Out with $Q^\top$ (dot products), back with $Q$ (linear combination) —
  two different operations, not two formulas
- Orthonormality is exactly $Q^\top Q = I$, so $Q^{-1} = Q^\top$: no inversion needed
- The two compulsory checks: **rebuild** the vector, and **compare lengths**
- Why choosing axes is half the job: sum-and-difference axes are what a *contrast*
  does, and they make the covariance diagonal

### Matrices as transformations

- A matrix as a machine that moves every point of space at once
- The **columns are where the axis arrows land**; $|\det A|$ is the area factor
- Rows to compute, columns to understand — the output is a linear combination of
  the columns, so the reachable set is exactly the span of the columns
- Order matters: $AB \neq BA$, and $(AB)^\top = B^\top A^\top$
- The **data matrix**: $X_{ij}$ is participant $i$, measure $j$ — and $Xw$ applies
  one scoring rule to everybody at once

## Materials

*Materials will appear here once uploaded.*

  To add materials: upload the PDFs to  assets/advanced/  using these names, then
  replace the line above with the links below (remove the surrounding comment):

  - 📊 [Slides]({{ '/assets/advanced/S1_Slides_Maths_training_Advanced_DEC_2026.pdf' | relative_url }})
  - ✏️ [Exercise sheet]({{ '/assets/advanced/Q_Ex1_Maths_training_Advanced_DEC_2026.pdf' | relative_url }})
  - ✅ [Solutions]({{ '/assets/advanced/Sol_Ex1_Maths_training_Advanced_DEC_2026.pdf' | relative_url }})
