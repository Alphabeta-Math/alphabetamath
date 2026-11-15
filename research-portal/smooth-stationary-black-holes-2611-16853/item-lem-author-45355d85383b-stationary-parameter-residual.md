---
title: Stationary parameter families have a decaying reference-slice residual
status: published
research_item: lem-author-45355d85383b-stationary-parameter-residual
dependency_level: 7
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [lem-author-45355d85383b-weighted-fifth-graph-derivative](item-lem-author-45355d85383b-weighted-fifth-graph-derivative)
- [lem-author-45355d85383b-smooth-mean-curvature-jet](item-lem-author-45355d85383b-smooth-mean-curvature-jet)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)
- [def-weighted-holder-spaces](item-def-weighted-holder-spaces)
- [lem-author-45355d85383b-stationary-maximal-flux-formula](item-lem-author-45355d85383b-stationary-maximal-flux-formula)
- [lem-author-45355d85383b-scaled-decay-holder-upgrade](item-lem-author-45355d85383b-scaled-decay-holder-upgrade)
- [lem-author-45355d85383b-weighted-products-and-derivatives](item-lem-author-45355d85383b-weighted-products-and-derivatives)
- [lem-author-45355d85383b-weighted-smooth-inversion](item-lem-author-45355d85383b-weighted-smooth-inversion)
- [lem-author-45355d85383b-relative-timelike-flow-chart](item-lem-author-45355d85383b-relative-timelike-flow-chart)
- [def-harrison-one-form](item-def-harrison-one-form)
- [def-harrison-one-form-family](item-def-harrison-one-form-family)
- [thm-stationary-harrison-primitive-input](item-thm-stationary-harrison-primitive-input)
- [thm-harrison-electrovacuum-construction-input](item-thm-harrison-electrovacuum-construction-input)
- [lem-author-84ac8de0c2f0-end-denominator-bounds](item-lem-author-84ac8de0c2f0-end-denominator-bounds)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:lem-taylor-integral-remainder](https://alphabetamath.cc/item/lem-taylor-integral-remainder)


## Statement

Work in ZFC and fix $0<\alpha<1$. Let $\Sigma_*$ be a supplied smooth embedded three-dimensional exterior with compact smooth boundary, a fixed end chart $x$ with $r=|x|>r_0$, and the fixed compact-core charts defining the global norms $C^{k,\alpha}_\beta(\Sigma_*)$. Let $(g_q,N_q,T)$ be stationary Lorentzian data on a common neighborhood of $\Sigma_*$, jointly smooth in the parameter and ambient coordinates, with one stationary field $T$ and smoothly varying time orientation $N_q$, for $q$ in an open real interval $I_0$ containing $q_*$. On a common stationary product end $\mathbb R_t\times\{x:r>r_0\}$ use fixed coordinates $(t,x)$ with $T=\partial_t$ future timelike, metric coefficients independent of $t$, and $\Sigma_*:\ t=u_*(x)$. The product spatial chart agrees with the fixed end chart, and the complement of this graph end in $\Sigma_*$ is compact. Suppose $b(q),c(q)>0$ are smooth and, on every compact subinterval of $I_0$, for $j=0,1$ there are common radii and constants giving
$$\partial_q^j(g_{q,00}+c(q)^2)=O_5(r^{-1}),\qquad \partial_q^j(g_{q,ij}-b(q)^2\delta_{ij})=O_5(r^{-1}),\qquad \partial_q^j g_{q,0i}=O_5(r^{-2}).$$
Write $e_{q,00}=g_{q,00}+c(q)^2$, $e_{q,ij}=g_{q,ij}-b(q)^2\delta_{ij}$ and $e_{q,0i}=g_{q,0i}$. Require also that $q\mapsto(e_{q,00},e_{q,ij})$ is $C^1$ in the annular $C^{4,\alpha}_{-1}$ norm and $q\mapsto e_{q,0i}$ is $C^1$ in the annular $C^{4,\alpha}_{-2}$ norm. These specify the parameter regularity needed here. A sufficient alternative is the same common differentiated bounds also for $j=2$; no second parameter derivative is otherwise required. Pointwise smoothness in $q$ alone is not substituted for this uniform norm control.

Assume $\Sigma_*$ is spacelike and maximal for $g_{q_*}$, and that its smooth end height satisfies $|D^j u_*|\le Cr^{-3/4-j}$ for $0\le j\le4$. Then on the end $u_*\in C^{5,\alpha}_{-3/4}$ and $\Delta_0u_*\in C^{2,\alpha}_{-3}$, where $\Delta_0$ is the Euclidean Laplacian in $x$.

There is an open interval $I$ with $q_*\in I\subset I_0$ on which this same reference hypersurface remains spacelike. Choose a fixed admissible transverse flow chart $F_w$ along $\Sigma_*$, with $F_0$ its inclusion and with flow field $Y=T$ on a distant end. For each $q\in I$, let $\mathcal H(q,w)$ be the mean curvature for $g_q$ pulled back by $F_w$, using the future normal and the sign $K(V,W)=g_q(\nabla_Vn,W)$. Thus $\mathcal H(q,0)$ is a function on the fixed $\Sigma_*$, independent of the auxiliary field at $w=0$. Then $q\mapsto\mathcal H(q,0)$ is $C^1$ into the global space $C^{2,\alpha}_{-3}(\Sigma_*)$, and $\mathcal H(q_*,0)=0$. The neighborhood is local about $q_*$; spacelikeness on an entire larger parameter interval is not asserted.

The Harrison application uses exactly the mass-one GR/SBS and original maximal-slice hypotheses recorded in the mathematical stationary-primitive and regular-construction suppliers, including their original stationary end, normalized Ernst potential and single chosen smooth normalized primitive $W_0$. For their metric family in the fixed original coordinates, all the stated mixed bounds and parameter-norm conditions hold on every compact $J\subset(0,1]$, with $b(q)=q$ and $c(q)=d_q/(4q)$. Around any positive reference parameter with a supplied maximal slice as above, the preceding conclusion therefore applies. At $q_*=1$ the metric formulas extend smoothly to a common neighborhood of the reference slice for $q$ slightly greater than $1$, with the same mixed bounds and a smaller admissible $I$ if necessary. This endpoint extension concerns the metric and its analytic mean-curvature map; no Einstein–Maxwell or electromagnetic-field assertion beyond $[0,1]$ is made.

## Statement references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[lem-author-45355d85383b-weighted-fifth-graph-derivative](item-lem-author-45355d85383b-weighted-fifth-graph-derivative)

[lem-author-45355d85383b-smooth-mean-curvature-jet](item-lem-author-45355d85383b-smooth-mean-curvature-jet)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[def-weighted-holder-spaces](item-def-weighted-holder-spaces)

[lem-author-45355d85383b-stationary-maximal-flux-formula](item-lem-author-45355d85383b-stationary-maximal-flux-formula)

[lem-author-45355d85383b-scaled-decay-holder-upgrade](item-lem-author-45355d85383b-scaled-decay-holder-upgrade)

[lem-author-45355d85383b-weighted-products-and-derivatives](item-lem-author-45355d85383b-weighted-products-and-derivatives)

[lem-author-45355d85383b-weighted-smooth-inversion](item-lem-author-45355d85383b-weighted-smooth-inversion)

[lem-author-45355d85383b-relative-timelike-flow-chart](item-lem-author-45355d85383b-relative-timelike-flow-chart)

[def-harrison-one-form](item-def-harrison-one-form)

[def-harrison-one-form-family](item-def-harrison-one-form-family)

[thm-stationary-harrison-primitive-input](item-thm-stationary-harrison-primitive-input)

[thm-harrison-electrovacuum-construction-input](item-thm-harrison-electrovacuum-construction-input)

[lem-author-84ac8de0c2f0-end-denominator-bounds](item-lem-author-84ac8de0c2f0-end-denominator-bounds)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:lem-taylor-integral-remainder](https://alphabetamath.cc/item/lem-taylor-integral-remainder)

## Facts & Assumptions

[F0] Stationary Lorentzian data fix the signature, smooth time orientation, metric connection and stationary field; an end additionally requires the field to be future timelike. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[A1] ZFC, including the Axiom of Choice, is carried from the graph bootstrap, transverse-chart and regular-construction suppliers. It is used when invoking those suppliers in steps 1.1, 2.1 and 1.2. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The weighted fifth-derivative bootstrap gives $u\in C^{5,\alpha}_{-3/4}$ and $\Delta_0u\in C^{2,\alpha}_{-3}$ for its supplied maximal graph in a Minkowski-leading stationary end. [lem-author-45355d85383b-weighted-fifth-graph-derivative](item-lem-author-45355d85383b-weighted-fifth-graph-derivative)

[F2] Mean curvature is a smooth finite-jet expression on the open set of spacelike graph jets, with bounded derivatives on compact admissible sets. [lem-author-45355d85383b-smooth-mean-curvature-jet](item-lem-author-45355d85383b-smooth-mean-curvature-jet)

[F3] The differentiated $O_5$ notation and parameter-uniform convention use common Cartesian radii and constants. One extra pointwise spatial derivative gives uniform scaled Hölder control. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data) [lem-author-45355d85383b-scaled-decay-holder-upgrade](item-lem-author-45355d85383b-scaled-decay-holder-upgrade)

[F4] The flow-graph definition fixes the pullback, future normal and mean-curvature sign. The transverse-chart supplier gives a fixed chart with $Y=T$ on the end once its uniform spacelike and coefficient bounds hold. [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data) [lem-author-45355d85383b-relative-timelike-flow-chart](item-lem-author-45355d85383b-relative-timelike-flow-chart)

[F5] The global weighted space uses the fixed compact-core norm plus scaled annuli; weighted differentiation, multiplication, positive inversion and smooth coefficient compositions obey the stated uniform Hölder estimates. [def-weighted-holder-spaces](item-def-weighted-holder-spaces) [lem-author-45355d85383b-weighted-products-and-derivatives](item-lem-author-45355d85383b-weighted-products-and-derivatives) [lem-author-45355d85383b-weighted-smooth-inversion](item-lem-author-45355d85383b-weighted-smooth-inversion)

[F6] The stationary flux supplier gives the exact normal and mean-curvature flux formula without a Minkowski-leading hypothesis; that hypothesis is needed only for its additional normalized end estimates. [lem-author-45355d85383b-stationary-maximal-flux-formula](item-lem-author-45355d85383b-stationary-maximal-flux-formula)

[F7] The mathematical primitive supplier, under its full mass-one GR/SBS and original maximality contract, supplies one stationary smooth $W_0$, normalized by $W_0(T)=d_0-D_0$, whose spatial end components are $O_5(r^{-3})$. The mathematical regular-construction supplier supplies the smooth metric family on the exterior and a common neighborhood of the bifurcation sphere, with $f<1$ on the exterior and $f\le0$ on that sphere. [thm-stationary-harrison-primitive-input](item-thm-stationary-harrison-primitive-input) [thm-harrison-electrovacuum-construction-input](item-thm-harrison-electrovacuum-construction-input)

[F8] The Harrison definitions specify $D_q=|1+q-(1-q)\sigma|^2$, $d_q=D_q(p)$ at the supplied pole $T(p)=0$, the polynomial family $W_q=(1-q)^2W_0-4q(1-q)T^\flat$, and the rank-one metric formula. They also give $W_q(T)=d_q-D_q$. [def-harrison-one-form](item-def-harrison-one-form) [def-harrison-one-form-family](item-def-harrison-one-form-family)

[F9] The mathematical end-denominator supplier uses the seed hypotheses $g_{00}=-1+2/r+O_6(r^{-2})$, $g_{0i}=O_6(r^{-2})$, $g_{ij}=\delta_{ij}+O_6(r^{-1})$ and proves $\sigma=1-2/r+O_6(r^{-2})$ and $d_q=(1+q)^2+(1-q)^2\psi(p)^2$. Its normalized-potential differential and end hypotheses are met by the original end and potential in F7. [lem-author-84ac8de0c2f0-end-denominator-bounds](item-lem-author-84ac8de0c2f0-end-denominator-bounds)

[F10] Taylor’s integral remainder applies to scalar smooth functions on parameter segments. We apply it componentwise, and to spatial derivatives and two-point differences before taking the weighted suprema. [math:lem-taylor-integral-remainder](https://alphabetamath.cc/item/lem-taylor-integral-remainder)

## Proof

**Given:** The fixed exterior, smooth metric family, mixed bounds and supplied reference maximal slice in the Statement; for the Harrison application use the complete contracts in F7.

**Goal:** Prove admissibility, the global residual estimate and parameter differentiability, and verify the Harrison mixed bounds and metric endpoint extension.

1.1 At the single fixed parameter $q_*$ set $s=c(q_*)t$ and $y=b(q_*)x$. These constant changes make $g_{q_*}$ Minkowski-leading, with differentiated errors of orders $-1,-1,-2$ through five derivatives. Its end graph has height $v(y)=c(q_*)u_*(y/b(q_*))$ and retains all the stated pointwise orders. Under A1 apply F1 in these normalized coordinates; the normalized flux hypotheses follow from the displayed metric bounds and F6. Constant dilations preserve the annular weights, and $\Delta_yv=(c(q_*)/b(q_*)^2)(\Delta_0u_*)(y/b(q_*))$. Rescaling back gives both asserted end estimates for $u_*$, in particular $p=Du_*\in C^{4,\alpha}_{-7/4}$. [given, A1, F1, F3, F5, F6, algebra]

1.2 For the Harrison application use F7 with all its recorded hypotheses, under A1. Its original stationary end and normalized potential meet F9, and its single primitive has the stated five spatial derivative bounds. Write $f=-g_{00}$ on that end, $\sigma=f+i\psi$ and $v_i=(W_q)_i$. The exact formulas in F8 give, for every real $q$ at which $D_q\ne0$, $$D_q=4q^2+e_q,\qquad v_i=(1-q)^2(W_0)_i-4q(1-q)g_{0i},\qquad (W_q)_0=d_q-D_q.$$ On every bounded parameter interval, finite polynomial differentiation gives $\partial_q^j e_q=O_5(r^{-1})$ and $\partial_q^j v_i=O_5(r^{-2})$ for every fixed finite $j$, with common constants. Indeed $1+q-(1-q)\sigma=2q+(1-q)(1-\sigma)$, and $1-\sigma=O_6(r^{-1})$ by F9; the square modulus is a polynomial in these fixed spatial fields and in $q$. The seed metric and $W_0$ have no $q$ dependence. No spatial decay is being inferred merely from rational parameter dependence. [A1, F7, F8, F9, algebra]

2.1 First choose a compact parameter interval about $q_*$ inside $I_0$; there $b,c$ are bounded above and away from zero. On the distant end the metric induced on the fixed graph is $$h_{q,ij}=g_{q,ij}+g_{q,0i}u_{*,j}+g_{q,0j}u_{*,i}+g_{q,00}u_{*,i}u_{*,j}=b(q)^2\delta_{ij}+O(r^{-1})$$ uniformly in $q$, since $Du_*=O(r^{-7/4})$. Thus it has a common positive lower eigenvalue after increasing the end radius. On the complementary compact truncation, $h_{q_*}$ is positive definite; in finitely many compact coordinate patches its minimum on unit tangent vectors is positive, and joint continuity keeps at least half this bound after shrinking to an interval $I$ about $q_*$. Bounded coefficients, bounded slope and the displayed tail lower bound are precisely the uniform tail conditions of F4; its compact continuity condition follows from joint smoothness. Apply its chart construction under A1. Hence a single chart can be chosen on a smaller $I$, and the residual is defined there. This proves admissibility on both the core and the full end. [given, A1, F2, F4, step 1.1, algebra]

2.2 Fix $J=[a,b]\subset(0,1]$. Step 1.2 gives $D_q\ge2a^2$ on a common sufficiently distant end. On each complementary compact truncation of the reference slice, including its boundary, F7 gives positive $D_q$ on a common ambient neighborhood, so compactness of the parameter/truncation product gives a positive lower bound. For $d_q$ use the explicit formula in F9, which is bounded above and away from zero on $J$. The elementary identity $\partial_qD_q^{-1}=-D_q^{-2}\partial_qD_q$, iterated together with spatial differentiation, gives $$D_q^{-1}=(4q^2)^{-1}+O_5(r^{-1})$$ with the same statement for each of the first two parameter derivatives of the error. For example subtract the leading inverse as $-e_q/(4q^2D_q)$; every differentiated error product still contains an error factor, while its denominators and their inverse derivatives are uniformly bounded at their proper spatial orders. All corresponding core derivatives are bounded by smoothness and the lower bound. These are exactly the quantitative denominator controls needed for mixed estimates. [F5, F7, F9, step 1.2, algebra]

3.1 Write inverse components as $g_q^{\mu\nu}$ and let $J_q=\sqrt{-\det g_q}$. On the end define $$Q_q(x,p)=-g_q^{00}+2g_q^{0i}p_i-g_q^{ij}p_ip_j,\qquad P_q^i(x,p)=\frac{J_q(g_q^{ij}p_j-g_q^{i0})}{\sqrt{Q_q(x,p)}}.$$ F6 gives $\mathcal H(q,0)=J_q^{-1}\partial_{x^i}P_q^i(x,Du_*)$. This uses its exact formula, valid for arbitrary stationary coefficients, rather than its extra Minkowski-leading estimates. The future sign is correct because $d(t-u_*)(T)=1$ and $T$ is future timelike by F0. On a common small slope ball on a distant end, $Q_q$ has a positive lower bound. Inverting the metric gives $g_q^{00}=-c(q)^{-2}+O_5(r^{-1})$, $g_q^{ij}=b(q)^{-2}\delta^{ij}+O_5(r^{-1})$ and $g_q^{i0}=O_5(r^{-2})$. For the mixed inverse entry use $g_q^{i0}=-g_q^{ij}g_{q,j0}/g_{q,00}$. Differentiating the inverse identity, this block identity and the determinant formula gives the same differentiated orders for the first parameter derivative of each error, and $J_q=c(q)b(q)^3+O_5(r^{-1})$. Positive denominator bounds and F3, F5 supply their uniform scaled Hölder estimates. Moreover these inverse and density errors are $C^1$ in the corresponding annular $C^{4,\alpha}$ norms: matrix inversion is the cofactor formula divided by a determinant bounded away from zero, and F5 applies to each finite product and smooth scalar composition. Subtracting the constant leading inverse or density leaves at least one original metric-error factor, by the componentwise segment identity in F10; its weight is preserved by F5. The mixed inverse identity preserves its stronger weight $-2$. [given, F0, F3, F5, F6, F10, step 2.1, algebra]

3.2 In the original stationary coordinates, substitute $(W_q)_0=d_q-D_q$ into the covariant metric formula in F8. It gives the exact component identities $$(g_q)_{00}=-\frac{f d_q^2}{4D_q},\qquad (g_q)_{0i}=\frac{d_q}{4}\left(g_{0i}-\frac{f}{D_q}v_i\right),\qquad (g_q)_{ij}=\frac14\left(D_qg_{ij}+g_{0i}v_j+g_{0j}v_i-\frac{f}{D_q}v_iv_j\right).$$ Using steps 1.2 and 2.2 and F9 yields $(g_q)_{00}=-d_q^2/(16q^2)+O_5(r^{-1})$, $(g_q)_{0i}=O_5(r^{-2})$ and $(g_q)_{ij}=q^2\delta_{ij}+O_5(r^{-1})$. For the spatial block the last three products are $O_5(r^{-4})$, while $(D_q-4q^2)g_{ij}$ and $4q^2(g_{ij}-\delta_{ij})$ have order $-1$. Applying the finite product rule after zero, one or two parameter derivatives preserves each indicated order by steps 1.2 and 2.2. This proves the mixed bounds through $j=2$ with $b(q)=q$ and $c(q)=d_q/(4q)$ on every such $J$. They also establish the parameter-norm conditions: by F3 the second parameter derivatives of the errors are uniformly bounded in their annular $C^{4,\alpha}$ norms. F10 at orders zero and one gives, in each respective norm, $\|\partial_q e_{q+h}-\partial_q e_q\|\le C|h|$ and $\|e_{q+h}-e_q-h\partial_qe_q\|\le C|h|^2$. Apply the scalar formulas to spatial derivatives and two-point differences before taking suprema; local smoothness permits the finite parameter integrals. The same argument proves the sufficient alternative in the Statement. Thus the application supplies actual spatial and parameter estimates, without using a physical component-asymptotics item. [F3, F8, F9, F10, step 1.2, step 2.2, algebra]

4.1 Take $x$ derivatives at fixed $p$ when writing $s_q(x,p)=J_q^{-1}\sum_i\partial_{x^i}P_q^i(x,p)$ and put $a_q^{ij}=J_q^{-1}\partial_{p_j}P_q^i$. Differentiating explicitly gives $$a_q^{ij}(x,p)=\frac{g_q^{ij}}{\sqrt{Q_q}}+\frac{(g_q^{ik}p_k-g_q^{i0})(g_q^{j\ell}p_\ell-g_q^{j0})}{Q_q^{3/2}}.$$ At the constant leading metric and zero slope this is $C(q)\delta^{ij}$ with $C(q)=c(q)b(q)^{-2}$. The difference at slope $p$ is bounded, with its finite scaled derivatives, by the metric error of order $r^{-1}$ plus terms of order $|p|^2+r^{-2}|p|+r^{-4}$; the absence of a leading linear slope term follows directly from the displayed formula and $g^{i0}=0$ in the leading metric. Also $$f_q(x)=s_q(x,0)=-J_q^{-1}\partial_{x^i}\left(\frac{J_q g_q^{i0}}{\sqrt{-g_q^{00}}}\right)$$ has weighted order $-3$, because $g_q^{i0}$ has order $-2$. Define $G_q^j(x,p)=\int_0^1\partial_{p_j}s_q(x,\theta p)\,d\theta$. The fixed-$p$ spatial derivative in $s_q$ differentiates a metric coefficient, density or conormal factor; a derivative of a constant leading coefficient vanishes. Thus every term of $\partial_p s_q$ has a spatial metric derivative bounded by $O(r^{-2})$, with mixed-component derivatives even smaller, and bounded smooth remaining factors. Consequently, after composition with $p=Du_*$, F3 and F5 give $E_q^{ij}=a_q^{ij}(x,Du_*)-C(q)\delta^{ij}\in C^{2,\alpha}_{-1}$, $G_q(x,Du_*)\in C^{2,\alpha}_{-2}$ and $f_q\in C^{2,\alpha}_{-3}$ on the end. Each of these three coefficient families is $C^1$ in its indicated annular norm. For $E_q$, subtract its value at the leading constant metric and zero slope by the finite-dimensional segment formula: metric-error factors have weight $-1$, and the remaining slope factors have weight at most $-7/4$, hence also include in weight $-1$. The sharper displayed quadratic slope estimate gives the same bound. For $G_q$, every term contains a spatial derivative of a metric error, of weight at most $-2$; its smooth coefficient factors are in weight zero. For $f_q$, expand the displayed derivative: either it differentiates $g^{i0}$, of weight $-3$, or it multiplies $g^{i0}$ of weight $-2$ by a derivative of a zero-weight coefficient, of weight at most $-2$. Step 3.1 and F5 now give $C^1$ dependence of these finite products and compositions in their weighted norms. The fixed reference jets are controlled by step 1.1 and have no parameter dependence. The integral identity for $s_q(x,p)-s_q(x,0)$ follows from F10. Its slope-parameter integrands and their derivatives have the same bounds and a common continuity modulus on $0\le\theta\le1$; differentiation and two-point differences can therefore be taken before these ordinary scalar integrals and their annular suprema. [F3, F5, F6, F10, step 1.1, step 3.1, algebra]

5.1 The total derivative in the flux formula now gives the precise decomposition $$\mathcal H(q,0)=C(q)\Delta_0u_*+E_q^{ij}u_{*,ij}+G_q^j(x,Du_*)u_{*,j}+f_q.$$ The first term is $C^1$ into $C^{2,\alpha}_{-3}$ by step 1.1 and smoothness of $C(q)$. The two height-error terms have weights $-1-11/4=-15/4$ and $-2-7/4=-15/4$, respectively. By F5 and step 4.1 they are $C^1$ into that weight, which includes continuously into weight $-3$. The last term is $C^1$ into weight $-3$ directly. On the compact core, F2 applies on the uniformly spacelike jets from step 2.1; joint smoothness bounds all required spatial and parameter derivatives in finitely many fixed charts. The scalar Taylor formulas in F10, applied also to derivatives and two-point differences, show $C^1$ dependence in the core $C^{2,\alpha}$ norm. Combining the core remainder and derivative-continuity bounds with the uniform annular bounds proves $C^1$ in the global norm: its definition is the sum of the fixed core norm and the annular supremum. Maximality at $q_*$ gives $\mathcal H(q_*,0)=0$. [F1, F2, F5, F10, step 1.1, step 2.1, step 4.1, algebra]

6.1 At $q=1$, $D_1=4$ everywhere and $d_1=4$. On the distant end the fixed seed fields and their recorded derivatives are bounded, so the polynomial estimates of step 1.2 hold also on a bounded interval about $1$ and keep $D_q$ positive there after shrinking it. On a compact ambient neighborhood of the remaining reference slice, smoothness and $D_1=4$ give the same positivity on a smaller common interval. The formulas for $W_q(T)=d_q-D_q$ and $d_q=(1+q)^2+(1-q)^2\psi(p)^2$ are polynomial identities, so remain valid slightly beyond $1$, with $d_q>0$. The rank-one map $A_qv=v+D_q^{-1}W_q(v)T$ has inverse $v\mapsto v-d_q^{-1}W_q(v)T$, and $g_q=(D_q/4)A_q^*g$ is Lorentzian there. Thus the rational metric formulas are jointly smooth across the endpoint; step 3.2 still gives their mixed end bounds, while smoothness controls the core. Apply steps 2.1, 3.1, 4.1 and 5.1 about any supplied reference maximal slice, shrinking $I$ for admissibility. This proves the endpoint analytic assertion without differentiating the electromagnetic square-root factor or extending any field equations. [F7, F8, F9, step 1.2, step 2.1, step 3.2, step 5.1, algebra] ∎
