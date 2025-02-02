

---
title: " High-Dimensional Volume and Concentration"
date: 2023-11-02T12:00:00-04:00
categories:
  - blog
tags:
  - Maths
  - probabilty


---


This repository explores geometric and probabilistic phenomena in high-dimensional spaces, including:
1. **Volume of a p-dimensional sphere** and its derivation using Beta/Gamma functions.
2. **Concentration of volume** near the equator and at the boundary.
3. **Gaussian distribution** in high dimensions and norm concentration.


# **1. Volume of a $p$-Dimensional Unit Sphere**

## **Definition**
The $p$-dimensional unit sphere $\mathcal{S}_p$ is defined as:
\[
\mathcal{S}_p = \left\{ \mathbf{x} \in \mathbb{R}^p : x_1^2 + x_2^2 + \dots + x_p^2 \leq 1 \right\}.
\]

## **Volume Derivation**
The volume $V_{\mathcal{S}_p}$ is computed recursively using polar coordinates and the Beta function:
1. **Recursive Integral**:
\[
V_{\mathcal{S}_p} = 2 \int_0^1 \left(1 - x_1^2\right)^{\frac{p-1}{2}} dx_1 \cdot V_{\mathcal{S}_{p-1}}.
\]
2. **Beta Function Substitution**:
   Using $t = x^2$, the integral becomes:
\[
\int_0^1 \left(1 - x^2\right)^{\frac{p-1}{2}} dx = \frac{1}{2} \beta\left(\frac{1}{2}, \frac{p+1}{2}\right),
\]
   where $\beta(z, w) = \frac{\Gamma(z)\Gamma(w)}{\Gamma(z+w)}$ is the Beta function.
3. **Final Formula**:
\[
V_{\mathcal{S}_p} = V_{\mathcal{S}_{p-1}} \cdot \frac{\Gamma\left(\frac{1}{2}\right)\Gamma\left(\frac{p+1}{2}\right)}{\Gamma\left(\frac{p}{2} + 1\right)}.
\]
   Solving recursively with $\Gamma(1/2) = \sqrt{\pi}$ and $V_{\mathcal{S}_2} = \pi$, we get:
\[
V_{\mathcal{S}_p} = \frac{\pi^{p/2}}{\Gamma\left(\frac{p}{2} + 1\right)}.
\]

# **2. Concentration of Volume Near the Equator**

## **Spherical Caps and Volume Ratio**
For a spherical cap at distance $\epsilon$ from the equator ($x_1 = 0$), the volume fraction is:
\[
\frac{2V(\epsilon)}{V_{\mathcal{S}_p}} = \frac{\int_\epsilon^1 \left(1 - x_1^2\right)^{\frac{p-1}{2}} dx_1}{\int_0^1 \left(1 - x_1^2\right)^{\frac{p-1}{2}} dx_1}.
\]

### **Asymptotic Analysis**
For large $p$, approximate $\left(1 - x_1^2\right)^{\frac{p-1}{2}} \approx e^{-\frac{p-1}{2}x_1^2}$:
\[
\frac{2V(\epsilon)}{V_{\mathcal{S}_p}} \approx \frac{\int_\epsilon^\infty e^{-\frac{p-1}{2}x^2} dx}{\int_0^\infty e^{-\frac{p-1}{2}x^2} dx} \leq \sqrt{\frac{2}{\pi(p-1)\epsilon^2}} e^{-\frac{\epsilon^2(p-1)}{2}}.
\]

### **Key Result**
For $\epsilon = \frac{c}{\sqrt{p-1}}$:
\[
1 - \frac{2V(\epsilon)}{V_{\mathcal{S}_p}} > 1 - \sqrt{\frac{2}{\pi c^2}} e^{-\frac{c^2}{2}}.
\]
**Interpretation**: Over 90% of the volume lies within $\mathcal{O}\left(\frac{1}{\sqrt{p}}\right)$ of the equator in high dimensions.



# **3. Concentration in an Annulus at the Boundary**

## **Volume of an Annulus**
The annulus $1 - \epsilon \leq \|\mathbf{x}\| \leq 1$ has volume:
\[
\text{Vol}_a(\epsilon) = V_{\mathcal{S}_p} \left[1 - (1 - \epsilon)^p\right].
\]

### **Exponential Decay**
For small $\epsilon$, $(1 - \epsilon)^p \approx e^{-p\epsilon}$:
\[
\frac{\text{Vol}_a(\epsilon)}{V_{\mathcal{S}_p}} \approx 1 - e^{-p\epsilon}.
\]
**Interpretation**: For $\epsilon = \frac{c}{p}$, nearly all volume concentrates in a thin shell of thickness $\mathcal{O}\left(\frac{1}{p}\right)$.



# **4. Gaussians in High Dimensions**

## **Norm Distribution**
For $\mathbf{x} \sim \mathcal{N}(0, \mathbf{I}_p)$, the norm $\|\mathbf{x}\|$ follows a chi distribution:
\[
f_{\|\mathbf{x}\|}(r) = \frac{1}{2^{p/2-1}\Gamma(p/2)} r^{p-1} e^{-r^2/2}.
\]

### **Mode and Concentration**
- **Mode**: $r^* = \sqrt{p - 1}$ (peak of the distribution).
- **Tail Probability**:
\[
\Pr\left(\left|\|\mathbf{x}\| - \sqrt{p}\right| > \epsilon\right) \leq \sqrt{2e} \cdot e^{-\epsilon^2/2}.
\]

**Interpretation**: Gaussian mass concentrates in a narrow annulus of radius $\sqrt{p} \pm \mathcal{O}(1)$.



# **Key Takeaways**
1. **Spheres**: 
   - Volume concentrates near the equator ($\sim \mathcal{O}(1/\sqrt{p})$) and surface ($\sim \mathcal{O}(1/p)$).
2. **Gaussians**:
   - Mass lies in a shell of radius $\sqrt{p}$, with negligible density near the origin.
3. **Tools**:
   - Beta/Gamma functions, Stirling’s approximation, and geometric intuition explain high-dimensional phenomena.



# **Usage**
All equations are written in LaTeX. Clone the repository and compile with LaTeX for detailed derivations.


