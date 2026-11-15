---
id: lem-author-29145f41e94d-smooth-weak-end-primitive
title: A smooth radial primitive can be returned to a weak end gauge
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-d20d145f998f-normalized-stationary-end
  - lem-author-d20d145f998f-decaying-time-gauge
  - lem-author-9e1b6fa65528-radial-exterior-primitive
  - def-author-9f9c6144aed8-ernst-mars-simon
  - lem-author-9e1b6fa65528-stationary-spatial-lifting
  - thm-vacuum-killing-ernst-input
  - def-stationary-asymptotic-decay-data
  - math:def-axiom-of-choice
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:thm-fundamental-theorem-of-riemannian-geometry
  - math:prop-christoffel-formula-for-the-levi-civita-connection
  - math:thm-christoffel-symbol-transformation-law
  - math:thm-chain-rule-for-total-derivatives
  - math:thm-algebra-of-derivatives
  - math:def-pullback-of-a-differential-form
  - math:thm-the-exterior-derivative-commutes-with-pullback
  - math:thm-the-exterior-derivative-squares-to-zero
  - physics:def-gr-smooth-lorentzian-objects
  - physics:def-gr-killing-field
  - physics:def-gr-metric-selected-connection
  - physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative
  - physics:def-gr-inverse-metric-and-musical-isomorphisms
  - math:def-oriented-smooth-manifold-and-oriented-chart
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:def-pullback-riemannian-metric
  - math:def-smooth-differential-k-form
  - math:def-closed-and-exact-differential-forms
  - math:def-interior-product-of-a-form-by-a-vector-field
  - math:def-exterior-derivative-by-the-invariant-vector-field-formula
  - math:def-wedge-product-of-differential-forms
  - math:def-lie-derivative-of-a-tensor-field
  - def-complex-self-dual-two-form-data
  - def-spacelike-maximal-hypersurface-data
dependency_roles:
  lem-author-d20d145f998f-normalized-stationary-end: mathematical-premise
  lem-author-d20d145f998f-decaying-time-gauge: mathematical-premise
  lem-author-9e1b6fa65528-radial-exterior-primitive: mathematical-premise
  def-author-9f9c6144aed8-ernst-mars-simon: mathematical-premise
  lem-author-9e1b6fa65528-stationary-spatial-lifting: mathematical-premise
  thm-vacuum-killing-ernst-input: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-complex-conjugate-real-imaginary-part-and-modulus: mathematical-premise
  math:thm-fundamental-theorem-of-riemannian-geometry: mathematical-premise
  math:prop-christoffel-formula-for-the-levi-civita-connection: mathematical-premise
  math:thm-christoffel-symbol-transformation-law: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:thm-algebra-of-derivatives: mathematical-premise
  math:def-pullback-of-a-differential-form: mathematical-premise
  math:thm-the-exterior-derivative-commutes-with-pullback: mathematical-premise
  math:thm-the-exterior-derivative-squares-to-zero: mathematical-premise
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  physics:def-gr-killing-field: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative: mathematical-premise
  physics:def-gr-inverse-metric-and-musical-isomorphisms: mathematical-premise
  math:def-oriented-smooth-manifold-and-oriented-chart: mathematical-premise
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:def-pullback-riemannian-metric: mathematical-premise
  math:def-smooth-differential-k-form: mathematical-premise
  math:def-closed-and-exact-differential-forms: mathematical-premise
  math:def-interior-product-of-a-form-by-a-vector-field: mathematical-premise
  math:def-exterior-derivative-by-the-invariant-vector-field-formula: mathematical-premise
  math:def-wedge-product-of-differential-forms: mathematical-premise
  math:def-lie-derivative-of-a-tensor-field: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 5
---

## Statement

Work in ZFC. Let a smooth oriented stationary Ricci-flat four-end of signature $(-,+,+,+)$ have an original stationary chart $(t,x)$ with $T=\partial_t$, $r=|x|$, $g_{00}=-1+2/r+O_6(r^{-2})$, $g_{0i}=O_6(r^{-2})$ and $g_{ij}=\delta_{ij}+O_6(r^{-1})$. The specified original section is $t=0$. Use $F_{ab}=\nabla_aT_b$ and a supplied smooth normalized Ernst potential $\sigma$, satisfying $d\sigma=2\iota_T(F+i\star_gF)$ and $\sigma\to1$ on this end. Put $f=\operatorname{Re}\sigma$ and $\psi=\operatorname{Im}\sigma$, so $\sigma=f+i\psi$; in this normalization $f=-g(T,T)$. Let $\Theta=4((f-1)F+\psi\star_gF)$ be smooth, closed and stationary, with $\iota_T\Theta=dD$ and $D=|1-\sigma|^2=O_6(r^{-2})$.

Take the auxiliary normalized stationary chart $(t',y)$ for the same $T$, supplied by end normalization, and write its smooth stationary transition as $y=q(x)$, $t'=t+F_*(x)$, with $R=|y|$. Its metric satisfies $g'_{00}=-1+2/R+O_\infty(R^{-2})$, $g'_{0a}=O_\infty(R^{-2})$ and $g'_{ab}=\delta_{ab}+O_\infty(R^{-1})$. Here $O_\infty$ means the differentiated estimate at every finite order. Assume the spatial coefficients of $\Theta$ in this auxiliary chart satisfy $\Theta'_{ab}=O_\infty(R^{-4})$. Then, on a sufficiently far end, for every real constant $c_0$ there is a smooth stationary one-form $W=(c_0-D)dt+w_i\,dx^i$ with $dW=\Theta$, $W(T)=c_0-D$ and $w_i=O_5(r^{-3})$. The original section is not replaced; any supplied maximality of that section is retained. The finite-order original bounds alone are not used to infer smoothness of an improper radial integral.

## Statement references

[[lem-author-d20d145f998f-normalized-stationary-end]]

[[lem-author-d20d145f998f-decaying-time-gauge]]

[[lem-author-9e1b6fa65528-radial-exterior-primitive]]

[[def-author-9f9c6144aed8-ernst-mars-simon]]

[[lem-author-9e1b6fa65528-stationary-spatial-lifting]]

[[thm-vacuum-killing-ernst-input]]

[[def-stationary-asymptotic-decay-data]]

[[math:def-axiom-of-choice]]

[[math:def-complex-conjugate-real-imaginary-part-and-modulus]]

[[math:thm-fundamental-theorem-of-riemannian-geometry]]

[[math:prop-christoffel-formula-for-the-levi-civita-connection]]

[[math:thm-christoffel-symbol-transformation-law]]

[[math:thm-chain-rule-for-total-derivatives]]

[[math:thm-algebra-of-derivatives]]

[[math:def-pullback-of-a-differential-form]]

[[math:thm-the-exterior-derivative-commutes-with-pullback]]

[[math:thm-the-exterior-derivative-squares-to-zero]]

[[physics:def-gr-smooth-lorentzian-objects]]

[[physics:def-gr-killing-field]]

[[physics:def-gr-metric-selected-connection]]

[[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative]]

[[physics:def-gr-inverse-metric-and-musical-isomorphisms]]

[[math:def-oriented-smooth-manifold-and-oriented-chart]]

[[math:def-riemannian-metric-and-riemannian-manifold]]

[[math:def-pullback-riemannian-metric]]

[[math:def-smooth-differential-k-form]]

[[math:def-closed-and-exact-differential-forms]]

[[math:def-interior-product-of-a-form-by-a-vector-field]]

[[math:def-exterior-derivative-by-the-invariant-vector-field-formula]]

[[math:def-wedge-product-of-differential-forms]]

[[math:def-lie-derivative-of-a-tensor-field]]

[[def-complex-self-dual-two-form-data]]

[[def-spacelike-maximal-hypersurface-data]]

## Facts & Assumptions

[F1] The mass-one weak metric bounds satisfy the end-normalization hypotheses; its auxiliary chart is for the same stationary field. The differentiated convention requires each Cartesian derivative of order $k$ to gain a factor $r^{-k}$ (or $R^{-k}$). Work in ZFC, carrying the normalization supplier's choice assumption; the local transition calculation below uses no additional choice principle. [[lem-author-d20d145f998f-normalized-stationary-end]] [[def-stationary-asymptotic-decay-data]] [[math:def-axiom-of-choice]]

[F2] The supplied normalized Ernst potential and Killing two-form use the stated complex-linear Hodge convention. The vacuum Ernst identity gives $\operatorname{Re}\sigma=-g(T,T)$ up to a real constant on a connected end; normalization fixes that constant to zero. Real and imaginary parts and modulus have their ordinary complex meanings. [[def-author-9f9c6144aed8-ernst-mars-simon]] [[thm-vacuum-killing-ernst-input]] [[math:def-complex-conjugate-real-imaginary-part-and-modulus]] [[def-complex-self-dual-two-form-data]]

[F3] For two charts of the same timelike stationary end whose quotient metrics are uniformly Euclidean-comparable and whose stationary connection covectors are $O(r^{-2})$ and $O(R^{-2})$, the unconditional time-gauge conclusion gives bounded $Dq,Dq^{-1}$, comparable radii and $dF_*=\varphi-q^*\varphi'$. No interior product or Cauchy hypothesis is required for that conclusion. [[lem-author-d20d145f998f-decaying-time-gauge]]

[F4] A smooth Riemannian metric has a unique Levi–Civita connection with $\Gamma^k_{ij}=\tfrac12h^{k\ell}(\partial_i h_{j\ell}+\partial_j h_{i\ell}-\partial_\ell h_{ij})$. The Christoffel transformation law applies to this same connection in overlapping smooth charts. [[math:thm-fundamental-theorem-of-riemannian-geometry]] [[math:prop-christoffel-formula-for-the-levi-civita-connection]] [[math:thm-christoffel-symbol-transformation-law]] Here a Riemannian metric is a smooth positive-definite symmetric covariant two-tensor; its pullback is $(q^*h')_x(v,w)=h'_{q(x)}(Dq_xv,Dq_xw)$. [[math:def-riemannian-metric-and-riemannian-manifold]] [[math:def-pullback-riemannian-metric]]

[F5] The total chain rule and the one-variable sum, product and quotient derivative rules apply componentwise and along coordinate lines to smooth functions and finite matrices. Reciprocal factors are used only where the denominator is bounded away from zero. [[math:thm-chain-rule-for-total-derivatives]] [[math:thm-algebra-of-derivatives]]

[F6] On a stationary product with $\iota_T\Theta=dD$ and stationary $D$, the form $\Theta-dt'\wedge dD$ descends to a smooth closed spatial two-form $b'$. A smooth spatial primitive $a'$ of $b'$ lifts to $W'=(c_0-D)dt'+a'$ with $dW'=\Theta$, stationarity and $W'(T)=c_0-D$. [[lem-author-9e1b6fa65528-stationary-spatial-lifting]]

[F7] A closed spatial two-form with coefficients $O_5(R^{-4})$ has the radial primitive with coefficients $O_5(R^{-3})$. If its differentiated bounds hold at every finite order, the same radial integral is smooth. [[lem-author-9e1b6fa65528-radial-exterior-primitive]]

[F8] Pullback of a one-form has coefficients $(q^*a')_i=a'_a(q(x))\partial_iq^a$. Exterior differentiation commutes with smooth pullback and satisfies $d^2=0$, so subtracting an exact smooth one-form preserves exterior derivative. [[math:def-pullback-of-a-differential-form]] [[math:thm-the-exterior-derivative-commutes-with-pullback]] [[math:thm-the-exterior-derivative-squares-to-zero]]

[F9] The smooth Lorentzian metric and Killing field have their geometric meanings; the orientation is a supplied smooth choice of tangent-space orientation. [[physics:def-gr-smooth-lorentzian-objects]] [[physics:def-gr-killing-field]] [[math:def-oriented-smooth-manifold-and-oriented-chart]] The connection is the torsion-free metric-compatible connection of $g$, and Ricci-flat means its Ricci tensor vanishes. [[physics:def-gr-metric-selected-connection]] Lower $T$ by $T^\flat=g(T,\cdot)$ and take its covariant derivative using the induced tensor derivative. [[physics:def-gr-inverse-metric-and-musical-isomorphisms]] [[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative]] Stationarity means vanishing Lie derivative along $T$; in the supplied stationary charts its flow translates time, so this is independence of the tensor coefficients from that time coordinate. [[math:def-lie-derivative-of-a-tensor-field]] If the original section is supplied as maximal, this means its mean curvature vanishes; retaining that same section retains the supplied property. [[def-spacelike-maximal-hypersurface-data]]

[F10] Smooth $k$-forms are smooth sections of $\bigwedge^kT^*M$; a form is closed when $d\omega=0$ and exact when $\omega=d\eta$. [[math:def-smooth-differential-k-form]] [[math:def-closed-and-exact-differential-forms]] Exterior differentiation is the invariant vector-field derivative on forms, and $\iota_T\omega$ inserts $T$ in the first slot; for complex forms use the complex-linear extension fixed in [F2]. [[math:def-exterior-derivative-by-the-invariant-vector-field-formula]] [[math:def-interior-product-of-a-form-by-a-vector-field]] The wedge in $dt'\wedge dD$ is the pointwise wedge of alternating covectors. [[math:def-wedge-product-of-differential-forms]]

## Proof

**Given:** The complete end, potential and two-form hypotheses in the Statement, in ZFC.

**Goal:** Construct the smooth stationary primitive with five differentiated decay bounds in the unchanged original chart.

1.1 The potential equation and alternation give $T(\sigma)=2T^aT^b\mathcal F_{ab}=0$, with $\mathcal F=F+i\star_gF$, so $D$ is stationary. The real-part identity in [F2] gives $f=-g(T,T)+C$ on the connected end. Since both $f$ and $-g(T,T)$ tend to one, $C=0$. Thus all scalar notation in $\Theta$ is fixed, and $D=(1-f)^2+\psi^2$. [given, F1, F2, F9, F10, algebra]

1.2 Restrict to a tail where $T$ is timelike. The stationary quotient metric has spatial representations $h_{ij}=g_{ij}-g_{0i}g_{0j}/g_{00}$ and $h'_{ab}=g'_{ab}-g'_{0a}g'_{0b}/g'_{00}$. The metric bounds and differentiation rules give $h=\delta+O_6(r^{-1})$ and $h'=\delta+O_\infty(R^{-1})$, hence both are uniformly Euclidean-comparable. The stationary connection covectors $\varphi_i=g_{0i}/g_{00}$ and $\varphi'_a=g'_{0a}/g'_{00}$ are respectively $O_6(r^{-2})$ and $O_\infty(R^{-2})$. They represent the same one-form $g(T,\cdot)/g(T,T)=dt+\varphi=dt'+\varphi'$, and $h=q^*h'$ represents the same quotient metric, independent of the choice of time section. All unconditional hypotheses of [F3] therefore hold: $Dq,Dq^{-1}$ are bounded and $R$ and $r$ are comparable. [given, F1, F3, F4, F5, F9]

2.1 Apply [F4] to the quotient metric of step 1.2. Its symbols obey $\Gamma=O_5(r^{-2})$ and $\Gamma'=O_\infty(R^{-2})$; the inverse-matrix estimates follow by repeated differentiation of $h^{-1}h=I$. The transformation law rearranges to $\partial_i\partial_jq^a=\Gamma^k_{ij}\partial_kq^a-\Gamma'{}^a_{bc}(q)\partial_iq^b\partial_jq^c$. Bounded first derivatives and comparable radii first give $D^2q=O(r^{-2})$. Inductively differentiate this identity $k$ times, $0\leq k\leq5$. Every term contains derivatives of $q$ through order at most $k+1$ and derivatives of a connection coefficient through order at most $k$. The induction estimates $D^jq=O(r^{-j})$ for $2\leq j\leq k+1$, together with bounded $Dq$, give at least one additional inverse power of $r$ for each differentiation. Thus every term is $O(r^{-k-2})$, and $D^{k+2}q=O(r^{-k-2})$. In particular all spatial transition derivatives through order seven are controlled without an interior completion or a change of section. [F4, F5, step 1.2]

2.2 In the auxiliary stationary product chart, [F6] supplies the descended smooth closed spatial form $b'$ from $\Theta-dt'\wedge dD$; its coefficients are the spatial coefficients $\Theta'_{ab}$. The assumed $O_\infty(R^{-4})$ bounds include the five differentiated bounds required by [F7] and its all-order hypothesis for smoothness. It gives one smooth $a'$ with $da'=b'$ and $a'_a=O_5(R^{-3})$. The lift from [F6] is $W'=(c_0-D)dt'+a'$, with $dW'=\Theta$, stationarity and $W'(T)=c_0-D$. No separate deduction of the assumed spatial decay from vacuum identities is needed here. [given, F6, F7, F10, step 1.1]

3.1 Equating the stationary connection one-forms gives $(dF_*)_i=\varphi_i-\varphi'_a(q(x))\partial_iq^a$. After $k\leq6$ derivatives, the chain and product rules use derivatives of $\varphi$ and $\varphi'$ through order $k$ and of $q$ through order at most $k+1\leq7$. The estimates of steps 1.2 and 2.1 give $\partial^k(dF_*)=O(r^{-2-k})$. Hence $dF_*=O_6(r^{-2})$ is a local consequence of the two end metrics, rather than an invocation of the global cutoff-extension theorem. [F3, F5, step 1.2, step 2.1]

4.1 Write $W'$ in the original chart and subtract $d(c_0F_*)$. This gives the smooth form $W=(c_0-D)dt+q^*a'-D\,dF_*$. By [F8], this subtraction preserves $dW=\Theta$; all its coefficients are stationary, and $dF_*(T)=0$, so $W(T)=c_0-D$. For $k\leq5$, differentiating $(q^*a')_i=a'_a(q(x))\partial_iq^a$ uses $a'$ derivatives through order $k$ and $q$ derivatives through order $k+1\leq6$. The five differentiated decay bounds of $a'$, comparable radii, bounded $Dq$ and the higher transition estimates give $\partial^k(q^*a')=O(r^{-3-k})$. The product rule and the assumed $D=O_6(r^{-2})$ give $D\,dF_*=O_5(r^{-4})$. Thus $w_i=O_5(r^{-3})$. Smoothness follows from the auxiliary smooth primitive and smooth transition; the original section remains $t=0$ throughout. [given, F5, F8, F9, F10, step 1.2, step 2.1, step 3.1, step 2.2] ∎
