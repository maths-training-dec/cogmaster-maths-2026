---
title: "Session 2 — Linear Algebra II"
layout: default
parent: Advanced track
nav_order: 2
---

# Session 2 — Linear Algebra II

The payoff session. Session 1 built vectors, spans and matrices; here we spend
that capital on the three questions people actually bring to a data table: *how
many dimensions does it really have?*, *which directions does a repeated linear
rule preserve?*, and *what varies together?* Rank, eigenvectors, PCA and the SVD
turn out to be one question asked four ways.

The same *participants × measures* table from Session 1 comes back throughout.

**Length:** ~120 min. Three frames are marked **[OPTIONAL]** and can be cut if the
slot is tight.

## Prerequisites

Session 1 — in particular span, linear independence, orthonormal bases, and
reading a matrix by its columns.

## Topics covered

### Determinant, inverse, rank

- The **determinant** as a signed area (volume) factor
- $\det = 0$ means a dimension is gone for good — and no inverse exists
- **Rank**: the honest count of dimensions, read off the span of the columns
- **Rank 1 at any size**: the outer product $uv^\top$ — one profile, one level per person
- Rank in practice: a total score alongside the items it is made of makes
  $X^\top X$ singular. Infinitely many weight vectors give identical predictions —
  this is **collinearity**
- *[Optional]* The inverse undoes it

### Eigenvectors and eigenvalues

- The directions that survive: $Av = \lambda v$, and why "nonzero" is load-bearing
- Finding them: one quadratic (the characteristic polynomial)
- **Diagonalization** $A = P\Lambda P^{-1}$ — work in the eigenbasis and powers
  become trivial
- Repeat the map enough times and the largest $|\lambda|$ wins
- **Complex eigenvalues mean rotation**
- *[Optional]* When diagonalization fails; where eigenvalues turn up

### Symmetric matrices, covariance, PCA

- Real symmetric $\Rightarrow$ real eigenvalues and *orthogonal* eigenvectors —
  this is precisely what makes PCA work
- The **covariance matrix**: what varies together
- **PCA** as the long axis of the cloud — the rotation Session 1 guessed by hand,
  now found automatically from the data
- How many components? Reading the spectrum

### Singular value decomposition

- $X = U\Sigma V^\top$ for **every** matrix — any shape, any rank, no exceptions
- What the three factors do: rotate, stretch, rotate
- SVD and PCA are the same theorem — PCA without ever forming the covariance matrix
- **Truncating**: the best small picture of a table

## Materials

*Materials will appear here once uploaded.*

<!--
  To add materials: upload the PDFs to  assets/advanced/  using these names, then
  replace the line above with the links below (remove the surrounding comment):

  - 📊 [Slides]({{ '/assets/advanced/S2_Slides_Maths_training_Advanced_DEC_2026.pdf' | relative_url }})
  - ✏️ [Exercise sheet]({{ '/assets/advanced/Q_Ex2_Maths_training_Advanced_DEC_2026.pdf' | relative_url }})
  - ✅ [Solutions]({{ '/assets/advanced/Sol_Ex2_Maths_training_Advanced_DEC_2026.pdf' | relative_url }})
-->
