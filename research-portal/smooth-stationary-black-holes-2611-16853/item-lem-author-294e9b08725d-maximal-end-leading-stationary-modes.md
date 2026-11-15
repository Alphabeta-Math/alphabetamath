---
title: Leading stationary modes and a spatial normalization of the same maximal end
status: draft
research_item: lem-author-294e9b08725d-maximal-end-leading-stationary-modes
dependency_level: 7
---

## Prerequisites

- [lem-author-294e9b08725d-maximal-end-same-slice-polyhomogeneous-gauge](item-lem-author-294e9b08725d-maximal-end-same-slice-polyhomogeneous-gauge)
- [thm-author-294e9b08725d-maximal-end-polyhomogeneous-input](item-thm-author-294e9b08725d-maximal-end-polyhomogeneous-input)
- [math:lem-pe18-spherical-harmonic-structure-and-density](https://alphabetamath.cc/item/lem-pe18-spherical-harmonic-structure-and-density)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Work in ZFC on the smooth stationary vacuum Lorentzian four-dimensional end supplied by the same-slice polyhomogeneous gauge lemma in [F1]. Retain its asymptotically horizontal maximal stationary slicing, with $T=\partial_\tau$ future timelike near infinity, $N\to1$, $X\to0$, and the same supplied CW maximal hypersurface at $\tau=0$. Write $h$, $k$, $N$ and $X$ for its induced metric, second form, lapse and shift, with $k=(2N)^{-1}\mathcal L_Xh$. Use the supplied asymptotically Cartesian quotient-harmonic spatial coordinates $y$, with $r=|y|$ and $\omega=y/|y|$, full differentiated polyhomogeneous expansions and $h-\delta,N-1,X=O_\infty(r^{-1})$. The normalized maximal vacuum KID identities are those supplied in [F2].

In the source spatial harmonic gauge, write the first coefficients as $N=1+r^{-1}n_1(\omega)+\cdots$, $X^i=r^{-1}A^i(\omega)+\cdots$, and $h_{ij}=\delta_{ij}+r^{-1}H_{ij}(\omega)+\cdots$. Then $n_1=-m$ is constant, A vanishes, and $H_{ij}=m(3\delta_{ij}-\omega_i\omega_j)$. The spatial radial change $z=y+(m/2)y/|y|$ preserves the same time coordinate and the same maximal slice and preserves full polyhomogeneity. In the resulting chart,
$$h_{ij}=\delta_{ij}+2m\delta_{ij}/r+O_\infty(r^{-2}\log^Jr),\quad N=1-m/r+O_\infty(r^{-2}\log^Jr),\quad X=O_\infty(r^{-2}\log^Jr),$$
with finite logarithmic powers at each retained order. The final spatial chart is not asserted still to be quotient-harmonic.

## Statement references

[lem-author-294e9b08725d-maximal-end-same-slice-polyhomogeneous-gauge](item-lem-author-294e9b08725d-maximal-end-same-slice-polyhomogeneous-gauge)

[thm-author-294e9b08725d-maximal-end-polyhomogeneous-input](item-thm-author-294e9b08725d-maximal-end-polyhomogeneous-input)

## Facts & Assumptions

[F1] The same maximal end has full differentiated expansions and order-minus-one initial lapse, shift and metric corrections in quotient-harmonic spatial coordinates. [lem-author-294e9b08725d-maximal-end-same-slice-polyhomogeneous-gauge](item-lem-author-294e9b08725d-maximal-end-same-slice-polyhomogeneous-gauge)

[F2] The normalized maximal vacuum KID system supplies div $X=0$, the lapse and vector equations and the stationary Ricci equation. [thm-author-294e9b08725d-maximal-end-polyhomogeneous-input](item-thm-author-294e9b08725d-maximal-end-polyhomogeneous-input)

[F3] The sphere Laplacian has constant kernel, degree-one eigenvalue minus two and the stated self-adjoint spectral decomposition. [math:lem-pe18-spherical-harmonic-structure-and-density](https://alphabetamath.cc/item/lem-pe18-spherical-harmonic-structure-and-density)

[F4] Work in ZFC, retaining the analytic choice assumptions inherited through [F1] and [F2]; the coefficient calculation and explicit radial map make no additional use of choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The supplied stationary vacuum maximal end, normalization, quotient-harmonic chart and differentiated expansions in the Statement and [F1]–[F2], working in ZFC as in [F4].

**Goal:** Prove the stated same-slice end consequence.

1.1 For a spherical function a, $\Delta_0(r^\sigma a)=r^{\sigma-2}(\Delta_{S^2}+\sigma(\sigma+1))a$. There are no log terms at order r to the power minus one, since the source O($r^{-1}$) bound forbids them. The maximal identity gives $k=(2N)^{-1}\mathcal L_Xh=O(r^{-2})$. In $\Delta_hN=N|k|^2$, the order $r^{-3}$ coefficient is therefore $\Delta_{S^2}n_1=0$, so $n_1=-m$. In the vector KID equation the order $r^{-3}$ coefficient likewise gives $\Delta_{S^2}A^i=0$ componentwise, so A is a constant vector. The order $r^{-2}$ coefficient in div $X=0$ is $-A\cdot\omega=0$, which forces $A=0$. [F1, F2, F3, given, algebra]

2.1 The stationary Ricci equation now has leading part $\operatorname{Ric}(h)_{ij}=\partial_i\partial_j(-m/r)+O(r^{-4}\log^Jr)$. The quotient metric differs from h only by a shift-square term, so its spatial harmonic condition gives the linearized h harmonic condition at order $r^{-2}$. The Ricci coordinate formula consequently gives $\Delta_{S^2}H_{ij}=2m(3\omega_i\omega_j-\delta_{ij})$. Since $\Delta_{S^2}(\omega_i\omega_j)=2\delta_{ij}-6\omega_i\omega_j$, all solutions have $H_{ij}=-m\omega_i\omega_j+C_{ij}$ for a constant symmetric matrix C. The linearized harmonic condition is $-C\omega+\tfrac12\operatorname{tr}(C)\omega-\tfrac32m\omega=0$, which gives $C=3m\delta$. [F1, F2, F3, step 1.1, algebra]

3.1 The map z is a spatial diffeomorphism sufficiently far out. Its inverse has $y=z-(m/2)z/|z|+O(r^{-1})$, whose leading derivative correction changes $m(3\delta-\omega\otimes\omega)/r$ to $2m\delta/r$. It leaves the leading lapse coefficient unchanged and cannot restore an absent $r^{-1}$ shift coefficient. The radial relation is exactly $|z|=|y|+m/2$, so substitution and the chain rule preserve integer-power/logarithmic expansions and all differentiated remainders. This is a spatial normalization after the source harmonic-gauge analysis; time and the slice have not changed. [F1, step 2.1, algebra] ∎
