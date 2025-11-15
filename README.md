# Parametric Curve Parameter Estimation

This repository contains the full solution to the problem of estimating the unknown
parameters of a nonlinear parametric curve using numerical optimization.  
The goal is to determine the values of:

- **θ** (rotation angle)
- **M** (exponential distortion factor)
- **X** (horizontal offset)

using only the provided `(x, y)` dataset sampled from the curve.

---

## 📌 Problem Overview

You are given the following parametric curve:

\[
x(t)=t\cos(\theta) - e^{M|t|}\sin(0.3t)\sin(\theta) + X
\]

\[
y(t)=42 + t\sin(\theta) + e^{M|t|}\sin(0.3t)\cos(\theta)
\]

Unknowns:

- \( \theta \in (0^\circ, 50^\circ) \)
- \( M \in (-0.05, 0.05) \)
- \( X \in (0,100) \)

Parameter \( t \) ranges from:

\[
6 < t < 60
\]

Given a CSV file containing **only x and y coordinates**, the task is to infer the best-fitting values
of the parameters.

---

## 📂 Repository Structure

