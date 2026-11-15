---
id: lem-annular-quasilinear-bootstrap-input
title: Uniform annular Schauder bootstrap for spacelike graph equations
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-db87cb8e0bab-annular-scaling
  - lem-author-db87cb8e0bab-stationary-flux-ellipticity
  - lem-author-db87cb8e0bab-divergence-gradient-holder
  - lem-author-db87cb8e0bab-coefficient-regularity
  - lem-author-db87cb8e0bab-linear-fourth-derivative-estimate
  - def-stationary-asymptotic-decay-data
  - def-normal-graph-and-mean-curvature-data
  - math:def-holder-spaces-c-k-alpha-and-their-scaled-norms
  - math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations
  - math:def-axiom-of-choice
  - math:thm-chain-rule-for-total-derivatives
  - math:lem-fundamental-theorem-of-calculus-for-banach-valued-continuous-curves
  - math:def-hk-and-hk-zero-notation
  - math:def-local-weak-solution-for-a-divergence-form-operator
  - math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle
  - math:lem-uniform-integral-error-bound
  - math:cor-mean-value-theorem
  - math:thm-divergence-theorem-for-bounded-c-one-euclidean-domains
dependency_roles:
  lem-author-db87cb8e0bab-annular-scaling: mathematical-premise
  lem-author-db87cb8e0bab-stationary-flux-ellipticity: mathematical-premise
  lem-author-db87cb8e0bab-divergence-gradient-holder: mathematical-premise
  lem-author-db87cb8e0bab-coefficient-regularity: mathematical-premise
  lem-author-db87cb8e0bab-linear-fourth-derivative-estimate: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  def-normal-graph-and-mean-curvature-data: mathematical-premise
  math:def-holder-spaces-c-k-alpha-and-their-scaled-norms: mathematical-premise
  math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:lem-fundamental-theorem-of-calculus-for-banach-valued-continuous-curves: mathematical-premise
  math:def-hk-and-hk-zero-notation: mathematical-premise
  math:def-local-weak-solution-for-a-divergence-form-operator: mathematical-premise
  math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle: mathematical-premise
  math:lem-uniform-integral-error-bound: mathematical-premise
  math:cor-mean-value-theorem: mathematical-premise
  math:thm-divergence-theorem-for-bounded-c-one-euclidean-domains: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
sources:
  references:
    - title: Xavier Fernández-Real and Xavier Ros-Oton, Regularity Theory for Elliptic
        PDE
      url: https://www.ub.edu/pde/xros/Llibre-ellipticPDE.pdf
      locator: Theorem 3.17, printed p. 93, PDF page 99 (zero-based page 98 in the
        currently retrieved 236-page PDF)
      statement: In dimension $d$, a scalar $z\in H^1(B_1)$ weakly satisfying
        $\operatorname{div}(B Dz)=0$, with measurable symmetric $\lambda_* I\le
        B\le\Lambda_* I$, obeys $\|z\|_{C^{0,\theta}(B_{1/2})}\le
        C\|z\|_{L^2(B_1)}$ for some $\theta>0$, with $C,\theta$ depending only
        on $d,\lambda_*,\Lambda_*$.
      hypotheses: Real scalar weak solution on a Euclidean unit ball; bounded
        measurable uniformly elliptic symmetric matrix. Applied after
        translation and dilation in dimension d=n+1 to the lifted homogeneous
        equation, with no lower-order terms.
      reading_limits: Read the complete extracted statement and immediate proof note
        of Theorem 3.17 on printed p. 93 in the author-hosted PDF during this
        assignment. The De Giorgi–Nash proof and its cited preceding results
        were not reconstructed. The lifting and finite-regularity application
        are local arguments here.
---

## Statement

Work in ZFC. Let $n\ge2$ be a fixed integer, $A=\{y\in\mathbb R^n:1/2<|y|<4\}$ and $A'=\{y\in\mathbb R^n:1<|y|<2\}$, and let $u_R$ be a family of smooth scalar graph heights on $RA$, for $R\ge R_0\ge1$. Indices $i,j$ range from $1$ to $n$, and repeated indices are summed. Set $v_R(y)=u_R(Ry)$ and $w_R=v_R/R$. Fix $0<\alpha<1$. The norms below are ordinary fixed-domain Hölder norms.

The general realized-coefficient version is as follows: if $a_R^{ij}(y)(v_R)_{ij}+b_R^j(y)(v_R)_j+c_R(y)v_R=f_R(y)$, the symmetric matrices $a_R$ have common positive ellipticity bounds, $a_R,b_R,c_R$ have common $C^{2,\alpha}$ bounds on $A$, and $\|f_R\|_{C^{2,\alpha}(A)}\le K/R$, then
$$\sum_{j=0}^4R^j\sup_{RA'}|D_x^ju_R|\le C(\sup_{RA}|u_R|+R^{-1}).$$

For a stationary spacelike maximal graph, with flux $P_R$ taking values in $\mathbb R^n$, the following explicit operator hypotheses supply those realized coefficient bounds, rather than assuming them from smoothness: $\operatorname{div}_yP_R(y,Dw_R)=0$, with no dependence on height; $|Dw_R|\le p_0$, $\|w_R\|_\infty\le M_0$; on the whole slope ball $|p|\le p_0$, $P_{R,p}$ is symmetric with $\lambda I\le P_{R,p}\le\Lambda I$ and $P_R$ has common joint $C^{4,\alpha}$ bounds on slightly larger slope neighborhoods. Write $s_R(y,p)=\sum_i\partial_{y_i}P_R^i(y,p)$, with partial derivatives at fixed $p$, and assume $\|s_R(\cdot,0)\|_{C^{2,\alpha}(A)}\le K/R^2$. Then the same estimate follows. Uniformity over additional parameters means common constants on the specified parameter set; no claim of uniformity at a degenerate parameter endpoint is made. The stationary Lorentzian four-manifold application uses $n=3$; its metric flux and sufficient background hypotheses are explicit in the flux lemma. Every application must verify these hypotheses, not only pointwise decay of the evaluated principal coefficients.

## Facts & Assumptions

[F1] The fixed-annulus rescaling and finite-cover identities hold. [[lem-author-db87cb8e0bab-annular-scaling]]

[F2] The explicit stationary Lorentzian flux has symmetric elliptic gradient derivative under its stated metric and spacelike-cone hypotheses. [[lem-author-db87cb8e0bab-stationary-flux-ellipticity]]

[F3] For a smooth flux under the gradient lemma's ellipticity, slope and flux-position-derivative hypotheses, the differentiated flux equation gives an initial gradient Hölder estimate before any Schauder application. [[lem-author-db87cb8e0bab-divergence-gradient-holder]]

[F4] Under its inherited smooth-flux hypotheses, the preliminary bootstrap gives common realized coefficient bounds using only structural data and a height bound for the normalized graph. [[lem-author-db87cb8e0bab-coefficient-regularity]]

[F5] The linear fourth-order estimate is linear in the height and the forcing once realized coefficient bounds are known. [[lem-author-db87cb8e0bab-linear-fourth-derivative-estimate]]

[F6] Uniform asymptotic estimates require a common chart, radius and constants. [[def-stationary-asymptotic-decay-data]]

[F7] The graph type, maximality convention and admissible spacelike image require explicit hypotheses. [[def-normal-graph-and-mean-curvature-data]]

[F8] Use ordinary Euclidean Hölder norms on the fixed annuli. [[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]]

[F9] In dimension $n\ge2$ and under Countable Choice, the interior Schauder estimate takes a bounded classical $C^2$ solution of a uniformly elliptic equation with controlled $C^{0,\gamma}$ coefficients and forcing to an interior $C^{2,\gamma}$ bound. Here $0<\gamma<1$; lower-order coefficients can be zero. [[math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations]]

[F10] Work in ZFC, carrying the analytic suppliers' choice assumptions. Full Choice supplies Countable Choice: for a sequence of nonempty sets, choose on its family of values and compose the choice function with that sequence. [[math:def-axiom-of-choice]]

[F11] For totally differentiable maps between open Euclidean sets, $D(G\circ\Phi)=DG(\Phi)D\Phi$. [[math:thm-chain-rule-for-total-derivatives]]

[F12] Under Countable Choice, a continuous Banach-valued curve on $[a,b]$ whose interior derivative extends continuously to $[a,b]$ satisfies $\varphi(b)-\varphi(a)=\int_a^b\varphi'(t)\,dt$. Use the real scalar case $X=\mathbb R$ and $[a,b]=[0,1]$. [[math:lem-fundamental-theorem-of-calculus-for-banach-valued-continuous-curves]]

[F13] Under Countable Choice, $H^1=W^{1,2}$ consists of square-integrable almost-everywhere classes with square-integrable first weak derivatives. For a bounded measurable uniformly elliptic real matrix $B$, the homogeneous local weak equation means $z\in H^1(U)$ and $\int_U(BDz)\cdot D\varphi=0$ for every $\varphi\in C_c^\infty(U)$. Use the real scalar convention with zero lower-order coefficients and datum. [[math:def-hk-and-hk-zero-notation]] [[math:def-local-weak-solution-for-a-divergence-form-operator]]

[F14] A continuous real integrand on a compact rectangle with a continuous parameter derivative may be differentiated through its Riemann integral. Apply twice, componentwise, with other spatial coordinates fixed. A uniform difference bound $\eta$ between integrable functions on $[0,1]$ bounds the difference of their integrals by $\eta$. [[math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle]] [[math:lem-uniform-integral-error-bound]]

[F15] The real mean value theorem applies to continuous functions on a closed interval differentiable in its interior. Along line segments, a bound on a derivative therefore bounds increments by the length times that bound. [[math:cor-mean-value-theorem]]

[F16] Under Countable Choice, for a bounded $C^1$ domain $U\subset\mathbb R^d$, $d\ge2$, and a vector field $V\in C^1(\overline U;\mathbb R^d)$, the divergence theorem gives $\int_U\operatorname{div}V=\int_{\partial U}V\cdot\nu$. In particular the integral is zero when $V$ vanishes near the boundary. [[math:thm-divergence-theorem-for-bounded-c-one-euclidean-domains]]

[F20] Use the homogeneous De Giorgi–Nash estimate recorded in External input, only after verifying the lifted weak equation in dimension $n+1$.

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the asserted estimate with the stated uniform dependence.

1.1 In the general realized-coefficient case apply [F5] to $v_R$ on $A$ with target annulus $A'$. It yields $\|v_R\|_{C^{4,\alpha}(A')}\le C(\|v_R\|_\infty+K/R)$. Rescale derivatives using [F1]. Thus the full original annular estimate follows whenever the stated coefficient hypothesis means actual $C^{2,\alpha}$ bounds as functions of position. [given, F1, F5, F8, F9, F10]

1.2 If $P_R$ is smooth, [F3] and [F4] give the preliminary coefficient bounds under the stated structural hypotheses. For a general jointly $C^{4,\alpha}$ flux, their smooth-flux interfaces are not invoked. Instead the following local argument extends the gradient and coefficient bootstrap to that finite regularity while keeping $w_R$ smooth, as already assumed. Choose a fixed finite sequence of nested annuli strictly between $A'$ and $A$, with room for all the successive interior estimates below. Work on balls with compact closures in the larger annuli, then cover the smaller ones using [F1]. All radii, separations and finite covering constants are fixed independently of $R$. Suppress $R$ in the local calculation. [given, F1, F3, F4, F8, F10]

1.3 On a convex ball, subtracting products gives $[fg]_{0,\gamma}\le\|f\|_\infty[g]_{0,\gamma}+\|g\|_\infty[f]_{0,\gamma}$ for $0<\gamma<1$; iterate for finite products. The identity $\Delta(fg)=f\Delta g+g\Delta f+\Delta f\Delta g$, divided by the increment and passed to the limit, gives the product derivative rule. By [F11] and [F15] on line segments, an outer map with bounded first derivatives is Lipschitz on the ball times the slope ball. Hence $[G\circ\Psi]_{0,\gamma}\le\operatorname{Lip}(G)[\Psi]_{0,\gamma}$. If $G$ is merely $\gamma$-Hölder and $\Psi$ is Lipschitz, instead use $[G\circ\Psi]_{0,\gamma}\le[G]_{0,\gamma}\operatorname{Lip}(\Psi)^\gamma$. These inequalities give the product and composition bounds used below. [F8, F11, F15, algebra]

1.4 For each coordinate $k$, put $z=w_k$, $a(y)=P_p(y,Dw(y))$ and $F(y)=-P_{y_k}(y,Dw(y))$, with the partial derivative at fixed slope. Differentiating the given flux equation gives $\operatorname{div}(aDz)=\operatorname{div}F$. This differentiation uses only two joint derivatives of $P$ and the assumed smoothness of $w$. In particular, $a$ is symmetric with $\lambda I\le a\le\Lambda I$, $|z|\le p_0$, and $|F|$ is bounded by the common structural bound. No uniform bound on $D^2w$ has been used. [given, F11, algebra]

2.1 On the chosen ball let $M=\|z\|_\infty+\|F\|_\infty$. If $M=0$, the gradient component is zero and needs no estimate. Otherwise define $Z(y,t)=z(y)/M+t$, $H(y)=F(y)/M$, and on the ball times $(-1,1)$ set $B=\begin{pmatrix}a&-H\\-H^T&1+2/\lambda\end{pmatrix}$. Since $|H|\le1$, its quadratic form is at least $(\lambda/2)|\xi|^2+|\tau|^2$, using $2|\tau H\cdot\xi|\le(\lambda/2)|\xi|^2+(2/\lambda)\tau^2$; an upper bound depends only on $\lambda,\Lambda$. Independence of $t$ gives $\operatorname{div}_{y,t}(BDZ)=\operatorname{div}_y(aDz/M-H)=0$. The entries are $C^1$ locally, so this identity is classical. On every ball $U$ with compact closure in the cylinder, $Z$ and its first derivatives are bounded on $\overline U$ and are square-integrable because $U$ is bounded. To check the weak identities, let $\varphi\in C_c^\infty(U)$ and $1\le\ell\le n+1$. The ball is a bounded $C^1$ domain in dimension $n+1\ge2$. Both $Z\varphi e_\ell$ and $\varphi BDZ$ are $C^1$ on a neighborhood of $\overline U$ and vanish near $\partial U$, since the coefficients are $C^1$ there and $\varphi$ has compact support in $U$. With Countable Choice supplied by [F10], [F16] and the product rule give $0=\int_U\operatorname{div}(Z\varphi e_\ell)=\int_U(Z\partial_\ell\varphi+\varphi\partial_\ell Z)$. These identities identify the classical derivatives as weak derivatives, so $Z\in H^1(U)$ by [F13]. Applying [F16] to the second field gives $0=\int_U\operatorname{div}(\varphi BDZ)=\int_U(BDZ)\cdot D\varphi+\int_U\varphi\operatorname{div}(BDZ)=\int_U(BDZ)\cdot D\varphi$. Thus [F13] verifies exactly the weak-solution hypotheses of [F20]. [step 1.4, F10, F13, F16, F20, algebra]

3.1 Apply [F20] after translation and dilation of the $(n+1)$-dimensional interior balls to unit balls. On the fixed cylinder $|Z|\le2$, so its $L^2$ norm on each such ball is uniformly bounded. Restrict the resulting estimate to $t=0$, multiply by the uniformly bounded $M$, and cover a smaller $y$ ball by finitely many such patches. Performing this for all $k$ gives a uniform $C^{0,\beta}$ bound for $Dw$. Decrease the exponent if necessary to ensure $0<\beta\le\alpha$ and $\beta<1$; on fixed bounded sets this costs only a diameter factor. The exponent and constants depend only on the structural data and fixed separations. [step 2.1, F1, F8, F10, F20, given]

4.1 Put $S(y)=s(y,Dw(y))$. The chain rule gives $a^{ij}w_{ij}=-S$. From step 3.1, the joint derivative bounds on $P$ and step 1.3, $a$ and $S$ have common $C^{0,\beta}$ bounds on interior balls. The matrix has the inherited ellipticity bounds, $w$ is smooth and bounded by $M_0$, both lower-order coefficients are zero, and [F10] supplies Countable Choice. Applying [F9] with exponent $\beta$ gives a uniform $C^{2,\beta}$ bound for $w$ on smaller balls. [step 1.3, step 3.1, F8, F9, F10, F11, given]

5.1 The chain and product rules with step 4.1 now give uniform $C^{1,\beta}$ bounds for $a$ and $S$. Differentiating the equation once yields $a^{ij}(w_k)_{ij}=-D_kS-(D_ka^{ij})w_{ij}$. Its right-hand side has a uniform $C^{0,\beta}$ bound by step 1.3, while $w_k$ is smooth and has a bounded supremum. Apply [F9] to each $w_k$ on smaller balls. This gives a uniform $C^{3,\beta}$ bound for $w$, without an assumed uniform bound on its third derivatives. [step 1.3, step 4.1, F8, F9, F10, F11, given, algebra]

6.1 Now $a$ and $S$ have uniform $C^{2,\beta}$ bounds, using joint derivatives of $P$ through order three and step 5.1. Twice differentiating the equation gives $a^{ij}(w_{k\ell})_{ij}=-D_{k\ell}S-(D_{k\ell}a^{ij})w_{ij}-(D_ka^{ij})w_{ij\ell}-(D_\ell a^{ij})w_{ijk}$. Every term on the right has a uniform $C^{0,\beta}$ bound; $w_{k\ell}$ is smooth with bounded supremum. Apply [F9] once more to obtain a uniform $C^{4,\beta}$ bound for $w$ on further smaller balls. The differentiated equations use only the existing finite derivatives of $P$; the classical $C^2$ membership needed in these applications comes from the given smoothness of $w$. All preliminary bounds may depend on $M_0$, without being linear in it. [step 1.3, step 5.1, F8, F9, F10, F11, given, algebra]

7.1 In particular all derivative suprema of $w$ through order four are uniformly bounded. By [F15], $Dw,D^2w,D^3w$ are uniformly Lipschitz on convex interior balls. For $0\le t\le1$ set $\Phi_t(y)=(y,tDw(y))$, $G(y,p)=P_p(y,p)$ and $H_j(y,p)=s_{p_j}(y,p)$. The maps $\Phi_t,D\Phi_t,D^2\Phi_t$ are uniformly bounded and Lipschitz. For either $J=G$ or $J=H_j$, [F11] twice gives $D^2(J\circ\Phi_t)=D^2J(\Phi_t)[D\Phi_t,D\Phi_t]+DJ(\Phi_t)D^2\Phi_t$. For $G$, joint derivatives through order two use derivatives of $P$ through order three; for $H_j$ they use derivatives of $P$ through order four. Their $\alpha$-Hölder bounds follow from the joint $C^{4,\alpha}$ hypothesis, using [F15] for lower derivatives. Thus step 1.3 gives a common $C^{2,\alpha}$ bound for $a=G\circ\Phi_1$ and for $h_j(y,t)=H_j(\Phi_t(y))$ uniformly in $t$. No fifth derivative of $P$ is used. [step 1.3, step 6.1, F8, F11, F15, given]

8.1 On closed coordinate boxes inside these balls, $h_j$ and its first two spatial derivatives are continuous jointly with $t\in[0,1]$, including at the boundary of the slope ball because $P$ is defined on a slightly larger slope neighborhood. By [F14], twice passing spatial derivatives through the integral gives $D_y^\nu b^j(y)=\int_0^1D_y^\nu h_j(y,t)\,dt$ for $|\nu|\le2$, where $b^j=\int_0^1h_j\,dt$. The uniform integral error bound in [F14] bounds the derivative suprema and the second-derivative $\alpha$-Hölder differences by the bounds of step 7.1. Finite interior covers assemble common $C^{2,\alpha}$ bounds for $a$ and $b$ on a fixed intermediate annulus: close pairs lie in a controlled ball, and separated pairs use twice the supremum divided by the fixed separation to the power $\alpha$, as in [F1]. This completes the finite-regularity coefficient bootstrap. [step 7.1, F1, F8, F14, given]

9.1 Apply [F11] to the composition $y\mapsto P_R(y,Dw_R(y))$ to expand the flux equation as $A_R:D^2w_R+s_R(y,Dw_R)=0$. For each fixed $y$, the curve $\varphi_y(t)=s_R(y,tDw_R(y))$ is continuous on $[0,1]$, and [F11] gives $\varphi_y'(t)=\sum_j(s_R)_{p_j}(y,tDw_R(y))(w_R)_j(y)$. This derivative extends continuously to both endpoints: the whole segment lies in the slope ball, and the assumed joint regularity holds on a neighborhood of it. Thus [F12], with Countable Choice supplied by [F10], gives $s_R(y,Dw_R)=s_R(y,0)+b_R\cdot Dw_R$. Multiplying by $R$ gives $A_R:D^2v_R+b_R\cdot Dv_R=-R s_R(y,0)$. The forcing has $C^{2,\alpha}$ norm at most $K/R$. On the intermediate annulus of step 8.1 the realized coefficients have common $C^{2,\alpha}$ bounds, so apply [F5] there with target $A'$ exactly as in step 1.1, and use [F1] to rescale back. The supremum on that intermediate annulus is bounded by $\sup_A|v_R|$. This proves the asserted linear height estimate. [step 1.1, step 8.1, F1, F5, F10, F11, F12, given, algebra]

10.1 For stationary metric applications, [F2] identifies the sufficient flux and zero-slope forcing assumptions; [F7] fixes what stationary flow graph and maximality mean, while [F6] states exactly what parameter uniformity requires. These interfaces do not establish that a particular spacetime satisfies the quantitative bounds: the consumer must check differentiated background estimates, the common spacelike slope neighborhood, stationarity and the zero-slope forcing. The estimate just proved applies whenever these checks hold. [F2, F6, F7, step 9.1] ∎

## External input

In dimension $d$, a scalar $z\in H^1(B_1)$ weakly satisfying $\operatorname{div}(B Dz)=0$, with measurable symmetric $\lambda_* I\le B\le\Lambda_* I$, obeys $\|z\|_{C^{0,\theta}(B_{1/2})}\le C\|z\|_{L^2(B_1)}$ for some $\theta>0$, with $C,\theta$ depending only on $d,\lambda_*,\Lambda_*$. This is the symmetric real scalar case of Theorem 3.17 in [Fernández-Real and Ros-Oton, Regularity Theory for Elliptic PDE](https://www.ub.edu/pde/xros/Llibre-ellipticPDE.pdf), printed p. 93 (current PDF page 99). Only this homogeneous estimate is imported as [F20]; its proof is not reconstructed. The differentiated equation, lifting and restriction steps supply the local application under finite flux regularity.

## Remarks

The original realized-coefficient estimate is retained. The added stationary-flux route supplies precise sufficient hypotheses for the intended graph application and separates preliminary nonlinear control from the final linear estimate. The original article is not cited as a prerequisite source. No claim about an error in that article is made.
