---
id: lem-author-a8fd09e77ebd-regular-kerr-analytic-chart
title: Analytic Kerr coordinates across the chosen nondegenerate horizon
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - math:def-real-analytic-germ-in-several-variables
  - def-stationary-lorentzian-data
  - math:def-lie-bracket-of-smooth-vector-fields
  - math:def-sine-and-cosine-by-power-series
  - math:lem-sine-and-cosine-series-converge-everywhere
  - math:thm-power-series-sums-are-real-analytic
  - math:thm-real-analytic-functions-closed-under-algebra-quotients-and-composition
  - math:cor-trigonometric-parity-and-pythagorean-identity
  - math:cor-pi-is-the-first-positive-sine-zero
  - physics:def-emg-causal-solution-and-horizon-vocabulary
dependency_roles:
  math:def-real-analytic-germ-in-several-variables: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  math:def-lie-bracket-of-smooth-vector-fields: mathematical-premise
  math:def-sine-and-cosine-by-power-series: mathematical-premise
  math:lem-sine-and-cosine-series-converge-everywhere: mathematical-premise
  math:thm-power-series-sums-are-real-analytic: mathematical-premise
  math:thm-real-analytic-functions-closed-under-algebra-quotients-and-composition: mathematical-premise
  math:cor-trigonometric-parity-and-pythagorean-identity: mathematical-premise
  math:cor-pi-is-the-first-positive-sine-zero: mathematical-premise
  physics:def-emg-causal-solution-and-horizon-vocabulary: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Ionescu–Klainerman, On the local extension of Killing vector-fields in
        Ricci flat manifolds
      url: https://arxiv.org/pdf/1108.3575
      locator: §3.1, equations (3.2)–(3.4) and the region R immediately after (3.4),
        printed/PDF pp. 15–16
      statement: Equation (3.2) is the Boyer–Lindquist Kerr metric; the coordinate
        substitution preceding (3.4) gives the displayed outgoing expression.
        Immediately after (3.4), the authors work on the region R with 2mr−q²>0
        and identify T=∂u. The broader outgoing-coordinate extension is
        justified locally below.
      hypotheses: 0<a<m. The source region R has 0<θ<π, r>0, −π<φ<π, u real and
        2mr−q²>0. The Boyer–Lindquist substitution is used locally where Δ≠0.
        The chosen horizon point is off the rotation axis and away from the
        bifurcation sphere.
      reading_limits: Consulted the PDF text of §3.1, equations (3.2)–(3.5) and the
        displayed definition of R, pp. 15–16. PDF screenshots were unavailable.
        Only the Kerr expression and coordinate substitution are imported; the
        analytic extension and symmetries are checked locally. No full
        maximal-extension atlas or independent vacuum-equation derivation is
        asserted.
dependency_level: 1
---

## Statement

Fix $0<a<m$ and local coordinates $(\theta,r,\varphi,u)$ on $D=(0,\pi)\times(0,\infty)\times(-\pi,\pi)\times\mathbb R$. Put $q^2=r^2+a^2\cos^2\theta$, $\Delta=r^2+a^2-2mr$ and $\Sigma^2=(r^2+a^2)^2-a^2\sin^2\theta\Delta$. Consider the outgoing Kerr expression

$$g=q^2d\theta^2-(du\otimes dr+dr\otimes du)+a\sin^2\theta(d\varphi\otimes dr+dr\otimes d\varphi)-\frac{2amr\sin^2\theta}{q^2}(d\varphi\otimes du+du\otimes d\varphi)+\frac{\Sigma^2\sin^2\theta}{q^2}d\varphi^2+\frac{2mr-q^2}{q^2}du^2.$$

It defines a real analytic Lorentzian metric on $D$, in the convergent multivariable power-series sense, and an outgoing-coordinate extension of the Boyer–Lindquist Kerr expression through $r=r_+=m+\sqrt{m^2-a^2}$. Ionescu–Klainerman §3.1 displays this formula and explicitly works on the smaller region $R=\{2mr-q^2>0\}\subset D$; the extension to $D$ is the local calculation below. Every off-axis point of $r=r_+$ lies in $R$. The coordinate fields $T=\partial_u$ and $Z=\partial_\varphi$ are commuting Killing fields. The formula is local and off the rotation axis; its denominators do not contain $\Delta$. No full maximal-extension atlas is claimed.

More precisely, put $H=\{r=r_+\}\subset D$, $B=r_+^2+a^2$, $q_H^2=r_+^2+a^2\cos^2\theta$, and $K=T+(a/B)Z$. The surface $H$ is a Killing horizon for this specified, nowhere-zero $K$. Its signed surface gravity, defined by the ambient covector equation $d(g(K,K))=-2\kappa_H K^\flat$ on $H$, is $\kappa_H=-(r_+-m)/B\ne0$. Here nondegenerate means that this scalar is nowhere zero. These are local Killing-horizon properties of the displayed metric.

## Statement references

[[math:def-real-analytic-germ-in-several-variables]]

[[math:def-sine-and-cosine-by-power-series]]

[[math:cor-pi-is-the-first-positive-sine-zero]]

[[def-stationary-lorentzian-data]]

[[math:def-lie-bracket-of-smooth-vector-fields]]

[[physics:def-emg-causal-solution-and-horizon-vocabulary]]

## Facts & Assumptions

[F1] The independent source gives the Boyer–Lindquist Kerr expression (3.2), the definitions (3.3), and the outgoing substitution $du=dt-(r^2+a^2)\Delta^{-1}dr$, $d\varphi=d\phi-a\Delta^{-1}dr$, producing (3.4). Its explicitly selected region after (3.4) is $R$, with $2mr-q^2>0$. This input does not assert that the source states a chart on all of $D$.

[F2] Sine and cosine mean their defining real power-series sums; both series converge absolutely for every real argument and hence have infinite radius. [[math:def-sine-and-cosine-by-power-series]] [[math:lem-sine-and-cosine-series-converge-everywhere]]

[F3] A power-series sum is real analytic at every point inside its radius interval, including every real point when the radius is infinite. A multivariable analytic germ is represented by an absolutely convergent local power series. [[math:thm-power-series-sums-are-real-analytic]] [[math:def-real-analytic-germ-in-several-variables]]

[F4] Real analytic functions on open real domains are closed under finite sums, products, compositions and quotients with nonzero denominators. [[math:thm-real-analytic-functions-closed-under-algebra-quotients-and-composition]]

[F5] The identities $\sin^2\theta+\cos^2\theta=1$ and $\sin\theta>0$ for $0<\theta<\pi$ hold. [[math:cor-trigonometric-parity-and-pythagorean-identity]] [[math:cor-pi-is-the-first-positive-sine-zero]]

[F6] Killing fields are defined by vanishing of the local-flow metric Lie derivative; the bracket acts as the commutator on smooth functions. [[def-stationary-lorentzian-data]] [[math:def-lie-bracket-of-smooth-vector-fields]]

[F7] A smooth embedded hypersurface is null when its induced metric has nonzero radical. It is a Killing horizon for a specified Killing field $K$ if its nonzero-generator part is nonempty and dense and $K$ is tangent and normal there. The signed surface gravity is defined there by the ambient covector equality $d(g(K,K))=-2\kappa_H K^\flat$. These are the conventions of Definition (b) of [[physics:def-emg-causal-solution-and-horizon-vocabulary]]. Here nondegenerate means that $\kappa_H$ is nowhere zero for the specified $K$.

## Proof

**Given:** The displayed expression, the coordinate domain $D$ and $0<a<m$.

**Goal:** Verify analytic regularity, the claimed Kerr-coordinate extension, the commuting symmetries and the nondegenerate Killing-horizon characterization.

1.1 By the defining series and their infinite radii, the power-series analyticity theorem applies to sine and cosine at every real $\theta_0$. Their expansions about $\theta_0$ also give multivariable germs by assigning exponent zero to the other coordinates; their absolute convergence is unchanged. The coordinate projections and constants have finite power-series expansions. [F2, F3]

2.1 The quantities $q^2$, $\Delta$, $\Sigma^2$ and all component numerators are finite sums and products of those analytic functions. Since $q^2\ge r^2>0$ on $D$, the quotient theorem applies everywhere on $D$ to the displayed components. Thus all components are real analytic, including at $\Delta=0$, and no denominator contains $\Delta$. [step 1.1, F4]

3.1 To verify that this analytic expression stays Lorentzian, write $s=\sin\theta$, $k=du-a s^2d\varphi$, $\ell=dr+a s^2d\varphi$, and $f=(2mr-q^2)/q^2$. Using $\sin^2\theta+\cos^2\theta=1$ gives $\Sigma^2=(r^2+a^2)q^2+2mra^2s^2$; substitution into the displayed expression yields $g=f k^2-(k\otimes\ell+\ell\otimes k)+q^2d\theta^2+q^2s^2d\varphi^2$. The forms $(k,\ell,d\theta,d\varphi)$ are a coframe, since $du=k+a s^2d\varphi$ and $dr=\ell-a s^2d\varphi$. Its first block is $\left(\begin{smallmatrix}f&-1\\-1&0\end{smallmatrix}\right)$, with eigenvalues $(f\pm\sqrt{f^2+4})/2$, one positive and one negative. The other two diagonal coefficients are positive because $q^2>0$ and $s>0$. Hence the metric has signature $(-,+,+,+)$ on all of $D$. The smooth field $N=\partial_u+(1+f^2)\partial_r/2$ has $g(N,N)=f-1-f^2=-(f-1/2)^2-3/4<0$, so it supplies a time orientation for the horizon conventions below. [F5, step 2.1, algebra]

4.1 On any radial interval where $\Delta\ne0$, choose local primitives $F'(r)=(r^2+a^2)/\Delta$ and $G'(r)=a/\Delta$ and set $t=u+F(r)$, $\phi=\varphi+G(r)$. The coordinate change has triangular Jacobian of determinant one. Substituting $du=dt-F'(r)dr$ and $d\varphi=d\phi-G'(r)dr$ in the outgoing expression gives $g=-\frac{q^2\Delta}{\Sigma^2}dt^2+\frac{\Sigma^2\sin^2\theta}{q^2}(d\phi-\frac{2amr}{\Sigma^2}dt)^2+\frac{q^2}{\Delta}dr^2+q^2d\theta^2$, exactly (3.2). Here $\Sigma^2=(r^2+a^2)q^2+2mra^2s^2>0$, so this comparison has no extra singular denominator. This is a local algebraic identification wherever $\Delta\ne0$, without a restriction on the sign of $2mr-q^2$. Steps 2.1 and 3.1 supply the regular outgoing-coordinate extension at the missing radial roots, rather than attributing that larger domain to the source's stated region $R$. [F1, F5, step 2.1, step 3.1, algebra]

4.2 The components are independent of $u$ and $\varphi$. Translation in either coordinate therefore preserves the metric locally, so the corresponding coordinate derivatives are Killing. Their commutator on every smooth function is zero because mixed coordinate derivatives commute. The proof makes no assertion about local Killing fields of a deformed metric. [F6, step 2.1, step 3.1]

5.1 At $r=r_+$, $\Delta=0$ and $2mr_+=r_+^2+a^2$, so $2mr_+-q^2=a^2\sin^2\theta>0$ off the axis. Thus every such horizon point is in the source region $R$, and the analytic regularity just proved applies across the chosen horizon there. [F5, step 2.1, step 4.1, algebra]

6.1 The level $H$ is a nonempty smooth embedded hypersurface, since $r$ is a coordinate and $dr\ne0$. The field $K=T+(a/B)Z$ is Killing: its local flow is $(u,\varphi)\mapsto(u+\tau,\varphi+(a/B)\tau)$, which preserves the components from step 4.2. It is tangent to $H$ and nowhere zero, since its $u$ component is one. At $H$, use $2mr_+=B$ and $q_H^2=B-a^2\sin^2\theta$ in the displayed metric to obtain $g(K,\partial_\theta)=g(K,\partial_u)=g(K,\partial_\varphi)=0$ and $g(K,\partial_r)=-1+(a^2/B)\sin^2\theta=-q_H^2/B$. Thus $K^\flat=-(q_H^2/B)dr$ as an ambient covector on $H$. In particular $K$ is a nonzero tangent vector orthogonal to every tangent vector of $H$, so the induced metric has nonzero radical and $H$ is null. Its nonzero-generator part is all of $H$, hence nonempty and dense. This verifies every Killing-horizon condition in [F7] on the time-oriented metric of step 3.1. [F7, step 3.1, step 5.1, step 4.2, algebra]

7.1 Keep $\Omega=a/B$ constant off $H$. Direct contraction of the displayed metric, using the Pythagorean identity, gives $g(K,K)=-\Delta(1-a\Omega\sin^2\theta)^2/q^2+\sin^2\theta((r^2+a^2)\Omega-a)^2/q^2$. On $H$, both $\Delta$ and $(r^2+a^2)\Omega-a$ vanish, while $1-a\Omega\sin^2\theta=q_H^2/B$. The differential of the squared second factor vanishes there; the differential of the first term is therefore $d(g(K,K))=-\Delta'(r_+)q_H^2B^{-2}dr$. This is an ambient differential: angular derivatives vanish because the norm restricts identically to zero on $H$, and the only remaining derivative is radial. Combining with $K^\flat=-(q_H^2/B)dr$ gives $\kappa_H=-\Delta'(r_+)/(2B)=-(r_+-m)/B$. Since $r_+-m=\sqrt{m^2-a^2}>0$ and $B>0$, the scalar is nowhere zero. The chosen outgoing branch and generator normalization account for its negative sign; nondegeneracy uses its nonvanishing. The extension through $H$ and its inclusion in $R$ remain those of steps 2.1–5.1. [F5, F7, step 5.1, step 6.1, algebra] ∎

## External input

The imported geometric expression is the Boyer–Lindquist formula (3.2) and its outgoing transformation (3.4) in the independent Ionescu–Klainerman paper, with the source's selected region $R$ recorded explicitly. Analyticity uses sine and cosine as power-series sums with infinite radii, analyticity of their sums at arbitrary real centers, their realization as multivariable analytic germs, and closure under finite sums, products and quotients with nonzero denominators. The Killing-horizon and signed-surface-gravity definitions are those of Definition (b) of [[physics:def-emg-causal-solution-and-horizon-vocabulary]]; nondegeneracy means nonvanishing of the specified scalar as stated in [F7]. Extension beyond $R$ and the horizon properties use the local calculations in Proof 3.1–4.1 and 6.1–7.1. The lemma as a whole has a local proof; no external-input flag or literature-derived proof provenance is claimed.
