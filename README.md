# Assignment-1: Learn Probability Density Functions using Roll-Number-Parameterized Non-Linear Model

## Objective
Transform the NO2 air quality feature using a personalized non-linear function, then fit a Gaussian-shaped probability density function (PDF) to the transformed data by estimating parameters **λ**, **μ**, and **c**.

---

## Dataset
- **Feature used:** NO2 (Nitrogen Dioxide)
- **Source:** [India Air Quality Data – Kaggle](https://www.kaggle.com/datasets/shrutibhargava94/india-air-quality-data)

---

## Requirements

| Library | Purpose |
|--------|---------|
| `numpy` | Numerical computation |
| `pandas` | Data loading and processing |
| `matplotlib` | Plotting and visualization |
| `scipy` | Statistical reference (optional) |

## Mathematical Summary

| Step | Formula |
|------|---------|
| Parameter a_r | `a_r = 0.05 × (r mod 7)` |
| Parameter b_r | `b_r = 0.3 × (r mod 5 + 1)` |
| Transformation | `z = x + a_r × sin(b_r × x)` |
| PDF Model | `p̂(z) = c × exp(−λ(z − μ)²)` |
| μ (mean) | `μ = mean(z)` |
| λ (precision) | `λ = 1 / (2 × var(z))` |
| c (scaling) | `c = 1 / sqrt(2π × var(z))` |

---

## 👤 Author
- **Roll Number:** *102303494*
- **Assignment:** 1 — PDF Estimation with Non-Linear Transformation
