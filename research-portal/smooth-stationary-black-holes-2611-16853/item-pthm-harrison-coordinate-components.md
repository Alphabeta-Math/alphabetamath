---
title: Coordinate components of the transformed metric
status: draft
research_item: pthm-harrison-coordinate-components
dependency_level: 3
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 10, §2.3, first display
      statement: In the original stationary coordinates the three displayed
        expressions give the 00, 0i and ij components of the Harrison metric.
      hypotheses: The article's stationary vacuum construction and the coordinates and
        parameter range stated in §2.
      reading_limits: Read the frozen article text at the cited display and its
        surrounding construction. This citation attributes the claim; the proof
        below uses the stated metric and one-form definitions.
---

PDF p. 10: ` §2.3, first display `

## Prerequisites

- [def-harrison-one-form](item-def-harrison-one-form)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [physics:def-gr-local-frame-and-tetrad-fields](https://alphabetamath.cc/physics/item/def-gr-local-frame-and-tetrad-fields)
- [math:def-tensor-product-of-multilinear-tensors](https://alphabetamath.cc/item/def-tensor-product-of-multilinear-tensors)


## Statement

Adopt the stationary vacuum model and regular stationary vacuum spacetime data, including the original maximal exterior section and mass-one normalization. Let $q\in[0,1]$, and suppose the Harrison one-form and metric are supplied on an open set $V$ where $D_q>0$. Thus $f=-g(T,T)$, $D_q=|q(1+\sigma)+(1-\sigma)|^2$, $d_q=D_q(p)$ at a supplied zero $p$ of $T$, and $W_q(T)=d_q-D_q$.

In an original stationary coordinate chart $(x^0,x^1,x^2,x^3)$ on $V$, meaning $T=\partial_0$ there, the transformed metric has components

$$(g_q)_{00}=-\frac{d_q^2f}{4D_q},\qquad (g_q)_{0i}=\frac{d_q}{4}\left(g_{0i}-\frac{f(W_q)_i}{D_q}\right),$$

$$(g_q)_{ij}=\frac14\left(D_qg_{ij}+g_{0i}(W_q)_j+g_{0j}(W_q)_i-\frac{f(W_q)_i(W_q)_j}{D_q}\right),\qquad i,j\in\{1,2,3\}.$$

## Statement references

[def-harrison-one-form](item-def-harrison-one-form)

[def-harrison-normalization](item-def-harrison-normalization)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[physics:def-gr-local-frame-and-tetrad-fields](https://alphabetamath.cc/physics/item/def-gr-local-frame-and-tetrad-fields)

[math:def-tensor-product-of-multilinear-tensors](https://alphabetamath.cc/item/def-tensor-product-of-multilinear-tensors)

## Facts & Assumptions

[A1] The stationary vacuum model and regular spacetime data are assumed, together with the specified maximal exterior section and mass-one convention. The component calculation is conditional on the supplied chart and fields. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-harrison-normalization](item-def-harrison-normalization)

[F1] Stationary Lorentzian data supply the metric $g$, its Killing field $T$, the metric dual $T^\flat=g(T,\cdot)$, and $f=-g(T,T)$. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] The Harrison normalization defines $D_q$ for the supplied potential. [def-harrison-normalization](item-def-harrison-normalization) The Harrison one-form definition sets $d_q=D_q(p)$ at the supplied zero $p$ of $T$. [def-harrison-one-form](item-def-harrison-one-form)

[F3] For the supplied one-form, $W_q(T)=d_q-D_q$, and $g_q=\tfrac14(D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-fD_q^{-1}W_q\otimes W_q)$ on $V$. [def-harrison-one-form](item-def-harrison-one-form)

[F4] A smooth chart supplies the coordinate frame $(\partial_0,\partial_1,\partial_2,\partial_3)$. We write $g_{ab}=g(\partial_a,\partial_b)$, $(g_q)_{ab}=g_q(\partial_a,\partial_b)$, and $\alpha_a=\alpha(\partial_a)$ for a one-form $\alpha$. [physics:def-gr-local-frame-and-tetrad-fields](https://alphabetamath.cc/physics/item/def-gr-local-frame-and-tetrad-fields)

[F5] For covectors $\alpha,\beta$ on the same tangent space, their tensor product satisfies $(\alpha\otimes\beta)(u,v)=\alpha(u)\beta(v)$. [math:def-tensor-product-of-multilinear-tensors](https://alphabetamath.cc/item/def-tensor-product-of-multilinear-tensors)

## Proof

**Given:** The model, data, parameter, supplied Harrison one-form and metric, positivity domain, and stationary coordinate chart in the Statement.

**Goal:** Calculate the three displayed component formulas.

1.1 Since $T=\partial_0$, the coordinate components satisfy $g_{00}=g(T,T)=-f$, $(T^\flat)_0=-f$, $(T^\flat)_i=g_{0i}$, and $(W_q)_0=W_q(T)=d_q-D_q$. Positivity of $D_q$ permits the displayed divisions. [given, F1, F3, F4]

2.1 Set $w=d_q-D_q$. Evaluating the tensor formula on $(\partial_0,\partial_0)$ gives $4(g_q)_{00}=-f(D_q+2w+w^2/D_q)=-fd_q^2/D_q$. Evaluating it on $(\partial_0,\partial_i)$ gives $4(g_q)_{0i}=(D_q+w)g_{0i}-f(1+w/D_q)(W_q)_i=d_q(g_{0i}-f(W_q)_i/D_q)$. [F3, F4, F5, step 1.1, algebra]

3.1 Evaluating the same tensor formula on $(\partial_i,\partial_j)$ gives the displayed spatial expression directly, because $(T^\flat)_i=g_{0i}$. These calculations prove all three formulas on the chart. [F3, F4, F5, step 1.1, step 2.1, algebra] ∎

## Source notes

The article citation attributes the component formulas. The proof is the local tensor expansion from the supplied Harrison definition; it does not use the article's assertion as a premise.
