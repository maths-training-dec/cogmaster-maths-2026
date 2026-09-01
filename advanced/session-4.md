---
title: "Session 4 — Analysis II"
layout: default
parent: Advanced track
nav_order: 4
---

# Session 4 — Analysis II

The second half of the analysis block, and the session where the linear algebra
of Sessions 1–2 pays off a second time. We add dimensions in three steps: several
inputs, then several outputs, then several equations running at once.

The recurring examples are the **error surface** of a fitted model (gradient
descent), a **mouse-tracking trajectory**, and a **two-accumulator decision model**.

**Length:** ~120 min, in three parts with a practice break in each.

## Prerequisites

Session 3 (derivatives, and $\dot x = ax + b$) and Session 2 (eigenvectors and
eigenvalues — Part C is essentially eigenvalues applied to motion).

## Topics covered

### A. Functions of several variables

- Several inputs, one output
- **Contour maps**: the only picture that scales past two dimensions
- **Partial derivatives**: vary one input, hold the others still
- The **gradient** — direction of steepest increase
- Where the gradient earns its keep: fitting a model, i.e. gradient descent on an
  error surface
- **Critical points**: where the gradient vanishes

### B. Vector-valued functions

- One input, several outputs
- A **trajectory** and its **velocity**: differentiate one component at a time
- Several inputs *and* several outputs: the **Jacobian**, the matrix of all
  partial derivatives — the local linear approximation of any smooth map

### C. Systems of differential equations

- From one equation to several: $\dot{\mathbf{x}} = A\mathbf{x}$
- Solving it: **one mode per eigenvector**
- **Stability, in one line**: the sign of the real parts of the eigenvalues
- The eigenvalues name the picture — node, saddle, spiral, centre
- A worked linear system, and **two accumulators making a decision**
- **Nonlinear systems**: linearise at a fixed point and reuse everything above
- **Nullclines** find the fixed points

## Materials

- 📊 [Slides]({{ '/assets/advanced/slides/S4_Slides_Maths_training_Advanced_DEC_2026.pdf' | relative_url }})
- ✏️ [Exercise sheet]({{ '/assets/advanced/exercises/Q_Ex4_Maths_training_Advanced_DEC_2026.pdf' | relative_url }})
