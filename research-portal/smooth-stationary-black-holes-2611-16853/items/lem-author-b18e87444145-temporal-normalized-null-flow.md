---
id: lem-author-b18e87444145-temporal-normalized-null-flow
title: Temporal normalization makes the null geodesic flow compact over compact bases
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves
  - math:thm-unique-maximal-integral-curve-through-each-point
  - math:thm-fundamental-theorem-on-flows
  - math:def-smooth-manifold
  - math:def-smooth-tensor-field
  - math:thm-sylvesters-law-of-inertia
  - math:def-affine-connection-on-a-smooth-manifold
  - math:def-geodesic-of-an-affine-connection
  - math:def-covariant-derivative-along-a-curve
  - math:def-lie-bracket-of-smooth-vector-fields
  - math:prop-leibniz-rules-for-the-lie-bracket-with-function-multiples
  - math:def-smooth-vector-bundle-rank-fibre-and-trivial-bundle
  - math:def-disk-bundle-sphere-bundle-and-thom-space
  - math:thm-the-tangent-bundle-has-a-canonical-smooth-2n-manifold-structure
  - math:def-induced-tangent-bundle-chart
  - math:def-countable-choice
  - math:def-smooth-vector-field-as-a-tangent-bundle-section
  - math:def-integral-curve-of-a-vector-field
dependency_roles:
  math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves: mathematical-premise
  math:thm-unique-maximal-integral-curve-through-each-point: mathematical-premise
  math:thm-fundamental-theorem-on-flows: mathematical-premise
  math:def-smooth-manifold: mathematical-premise
  math:def-smooth-tensor-field: mathematical-premise
  math:thm-sylvesters-law-of-inertia: mathematical-premise
  math:def-affine-connection-on-a-smooth-manifold: mathematical-premise
  math:def-geodesic-of-an-affine-connection: mathematical-premise
  math:def-covariant-derivative-along-a-curve: mathematical-premise
  math:def-lie-bracket-of-smooth-vector-fields: mathematical-premise
  math:prop-leibniz-rules-for-the-lie-bracket-with-function-multiples: mathematical-premise
  math:def-smooth-vector-bundle-rank-fibre-and-trivial-bundle: mathematical-premise
  math:def-disk-bundle-sphere-bundle-and-thom-space: mathematical-premise
  math:thm-the-tangent-bundle-has-a-canonical-smooth-2n-manifold-structure: mathematical-premise
  math:def-induced-tangent-bundle-chart: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:def-smooth-vector-field-as-a-tangent-bundle-section: mathematical-premise
  math:def-integral-curve-of-a-vector-field: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Assume countable choice. Let $(E,g)$ be a smooth time-oriented Lorentz manifold and $v$ a smooth temporal function with $dv$ positive on future causal vectors. Put $\mathcal N_v=\{(p,w):g_p(w,w)=0,\ dv_p(w)=1,\ w\text{ future}\}$. It is a smooth bundle of spheres over $E$, compact over each compact base subset. Unparametrized future null geodesics, parametrized by $v$, are precisely the base curves of a smooth vector field on $\mathcal N_v$. Its maximal flow domain is open and its flow is smooth. If a finite parameter-end portion of a lifted orbit remains over a compact base subset, it extends beyond that endpoint.

## Facts & Assumptions

[F1] Smooth vector fields have unique maximal integral curves, local smooth dependence, and open smooth maximal-flow domains. [[math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves]] [[math:thm-unique-maximal-integral-curve-through-each-point]] [[math:thm-fundamental-theorem-on-flows]] [[math:def-smooth-vector-field-as-a-tangent-bundle-section]] [[math:def-integral-curve-of-a-vector-field]]

[F2] Use smooth manifolds without boundary in any finite dimension $m$. Here a Lorentz metric is a smooth symmetric covariant two-tensor of inertia $(m-1,1,0)$. A tangent vector $w$ is timelike if $g(w,w)<0$, null if $w\ne0$ and $g(w,w)=0$, and causal if $w\ne0$ and $g(w,w)\le0$; the zero vector is neither null nor causal. Time orientation specifies one component of the timelike cone $\{w:g(w,w)<0\}$, and causal vectors in its closure are future. For a covector $\alpha$, define $\alpha^\sharp$ by $g(\alpha^\sharp,X)=\alpha(X)$ and $g^{-1}(\alpha,\beta)=g(\alpha^\sharp,\beta^\sharp)$. Write $\operatorname{grad}_g v=(dv)^\sharp$. Temporal means $g^{-1}(dv,dv)<0$, with the positive future sign imposed in the Statement. These conventions are dimension independent; Sylvester inertia identifies the positive and negative dimensions. [[math:def-smooth-manifold]] [[math:def-smooth-tensor-field]] [[math:thm-sylvesters-law-of-inertia]]

[F3] An affine connection is function-linear in its first field and obeys $\nabla_X(fY)=X(f)Y+f\nabla_XY$. Covariant differentiation along a curve is denoted $D_s$; an affine geodesic satisfies $D_s\gamma'=0$. An unparametrized future null geodesic means a nonconstant future null curve locally admitting an increasing affine-geodesic parametrization. Below we construct the torsion-free metric-compatible connection of $g$ in arbitrary dimension. Define its Hessian by $\operatorname{Hess}_g v(X,Y)=X(Yv)-dv(\nabla_XY)$. [[math:def-affine-connection-on-a-smooth-manifold]] [[math:def-geodesic-of-an-affine-connection]] [[math:def-covariant-derivative-along-a-curve]]

[F4] The bracket is $[X,Y]f=X(Yf)-Y(Xf)$, with $[X,fY]=f[X,Y]+X(f)Y$ and $[fX,Y]=f[X,Y]-Y(f)X$. [[math:def-lie-bracket-of-smooth-vector-fields]] [[math:prop-leibniz-rules-for-the-lie-bracket-with-function-multiples]]

[F5] For a smooth real vector bundle $H\to E$ with supplied positive-definite smooth fiber metric $h$, its sphere bundle is $S_h(H)=\{(p,e):h_p(e,e)=1\}$. Smooth orthonormal trivializations give its usual smooth sphere-bundle structure. The rank-zero sphere bundle is empty. Compactness and the required trivializations for the particular bundle below are proved locally. [[math:def-smooth-vector-bundle-rank-fibre-and-trivial-bundle]] [[math:def-disk-bundle-sphere-bundle-and-thom-space]]

[F6] Assume $\mathrm{AC}_\omega$ (countable choice). Under this hypothesis the tangent bundle $TE$ has its canonical smooth $2m$-manifold structure, with the induced tangent-bundle charts as a smooth atlas. For a smooth chart $x$ on $E$, its induced chart sends $w=\sum_i w^i\partial_{x^i}|_p$ to $(x(p),(w^1,\ldots,w^m))$; these are the tangent-bundle coordinates used below. [[math:def-countable-choice]] [[math:thm-the-tangent-bundle-has-a-canonical-smooth-2n-manifold-structure]] [[math:def-induced-tangent-bundle-chart]]

## Proof

**Given:** The hypotheses and dimension-independent conventions above.

**Goal:** Establish the sphere-bundle, flow, path and continuation assertions.

1.1 For smooth local fields put $K(X,Y,Z)=Xg(Y,Z)+Yg(X,Z)-Zg(X,Y)+g([X,Y],Z)-g([X,Z],Y)-g([Y,Z],X)$. Expanding the product rules gives $K(fX,Y,Z)=fK(X,Y,Z)$, $K(X,Y,fZ)=fK(X,Y,Z)$ and $K(X,fY,Z)=fK(X,Y,Z)+2X(f)g(Y,Z)$: the derivatives of $f$ from the bracket terms cancel those from the three metric derivatives, except the two copies of $X(f)g(Y,Z)$ in the last identity. Thus $K(X,Y,\cdot)$ is a covector. Nondegeneracy defines a unique $\nabla_XY$ by $2g(\nabla_XY,Z)=K(X,Y,Z)$. In a chart it is $\frac12\sum_{i,j}g^{ij}K(X,Y,\partial_j)\partial_i$, which is smooth: the inverse matrix entries are the adjugate entries divided by the nonzero determinant. The defining intrinsic identity makes these chart fields agree on overlaps. The three scalar identities and real bilinearity give precisely the affine-connection rules. [given, F2, F3, F4, F6, algebra]

1.2 Set $a=\sqrt{-g^{-1}(dv,dv)}>0$ and $n=-\operatorname{grad}_g v/a$. Then $g(n,n)=-1$, $dv(n)=a$, and the positive future sign makes $n$ future. The smooth projection $X\mapsto X+g(X,n)n$ has image $H=n^\perp=\ker dv$ and kernel $\mathbb Rn$. Projecting coordinate fields and selecting a locally independent $(m-1)$-tuple gives local smooth frames of $H$. The orthogonal splitting $TE=\mathbb Rn\oplus H$ and inertia imply $h=g|_H$ is positive definite. Applying Gram--Schmidt in each such frame is smooth since every normalization denominator is positive, and gives smooth orthonormal frames. Every nonzero future null vector is uniquely $w=b(n+e)$ with $b=-g(w,n)>0$, $e\in H$, and $h(e,e)=1$. Since $dv(w)=ab$, the map $(p,e)\mapsto(p,a^{-1}(n+e))$ is a smooth bundle isomorphism from $S_h(H)$ onto $\mathcal N_v$, with inverse $e=aw-n$. For any compact $B\subset E$, take finitely many closed compact subsets $B_i$ covering $B$, each contained in an orthonormal trivialization (shrink coordinate neighborhoods inside the trivializations first). The sphere bundle over each $B_i$ is $B_i\times S^{m-2}$, hence compact, so its finite union over $B$ is compact. The same holds for $\mathcal N_v$; no vector there is zero, since $dv(w)=1$. If $m=1$, $H$ has rank zero and $\mathcal N_v$ is empty, with all flow assertions vacuous. [given, F2, F5, F6, algebra]

2.1 Expansion of the same six terms gives $K(X,Y,Z)-K(Y,X,Z)=2g([X,Y],Z)$ and $K(X,Y,Z)+K(X,Z,Y)=2Xg(Y,Z)$. Consequently the connection is torsion-free and metric-compatible. Conversely those two properties, substituted into the six terms, give $K(X,Y,Z)=2g(\nabla_XY,Z)$, proving uniqueness. With indices ranging over all $1,\ldots,m$, evaluation on coordinate fields yields $\Gamma^i_{jk}=\frac12\sum_\ell g^{i\ell}(\partial_jg_{k\ell}+\partial_kg_{j\ell}-\partial_\ell g_{jk})$ and $(\operatorname{Hess}_g v)_{jk}=\partial_j\partial_kv-\sum_i\Gamma^i_{jk}\partial_i v$. In particular the coefficients and Hessian are smooth in every finite dimension, and $D_sw$ has components $(w^i)' +\sum_{j,k}\Gamma^i_{jk}(p)(p^j)'w^k$. This supplies the dimension-independent metric connection and geodesic equation needed here. [F2, F3, F4, step 1.1, algebra]

3.1 For $m\ge2$, define the lifted equation in each tangent-bundle chart by the following formula, where repeated indices are summed: [step 2.1, step 1.2]
$$ (p^i)\prime=w^i,\qquad (w^i)\prime=-\Gamma^i_{jk}w^jw^k-(\operatorname{Hess}_g v)(w,w)w^i. $$
Its intrinsic form is $D_sw=-(\operatorname{Hess}_g v)(w,w)w$, so the chart fields agree and are smooth. Write $H_v=(\operatorname{Hess}_g v)(w,w)$. The derivatives of the two constraints are $(dv(w))\prime=H_v(1-dv(w))$ and $(g(w,w))\prime=-2H_vg(w,w)$, using metric compatibility. They vanish on $\mathcal N_v$, so the field is tangent to its smooth constraint manifold; future direction is retained there by continuity and the nonzero normalization. Along its base curves $d(v(p))/ds=1$. [F3, F6, step 2.1, step 1.2, algebra]

4.1 To check the geodesic-path assertion, along a lifted orbit choose $\lambda(s)=\lambda(s_0)\exp(\int_{s_0}^s H_v(r)\,dr)>0$ and introduce $t$ by $dt/ds=1/\lambda(s)$. Then $dp/dt=\lambda w$ and $D_t(dp/dt)=\lambda(\lambda\prime-\lambda H_v)w=0$. This gives an increasing affine parameter locally. Conversely, for an affine future null geodesic $c(t)$ put $q=dv(c\prime)>0$ and use $s=v(c(t))$ as parameter. Then $w=c\prime/q$ and $dq/dt=(\operatorname{Hess}_g v)(c\prime,c\prime)$ give $D_sw=-(\operatorname{Hess}_g v)(w,w)w$ and $dv(w)=1$. Thus exactly the stated geodesic paths lift to this field, with the temporal parameter differing from the flow parameter by an additive constant. [given, F3, step 2.1, step 3.1, algebra]

5.1 Apply [F1] to the smooth field on $\mathcal N_v$. Its maximal flow domain is open and its flow is smooth. Suppose an orbit $z(s)$ has a finite right endpoint $b$ and its terminal portion has base in compact $B$. By step 1.2 that portion lies in compact $\mathcal N_v|_B$. At every point of this compact set, local existence gives a neighborhood and a flow defined for $|t|<\varepsilon_i$ uniformly on that neighborhood. Take a finite subcover and let $\varepsilon=\min_i\varepsilon_i>0$. Choose $s_0<b$ in the terminal portion with $b-s_0<\varepsilon/2$. A neighborhood containing $z(s_0)$ supplies a solution until $s_0+\varepsilon>b$; uniqueness glues it to the original orbit. This contradicts maximality. Reversing the parameter handles a finite left endpoint. This is continuation in temporal time and asserts no global affine completeness. [F1, step 1.2, step 3.1, step 4.1] ∎
