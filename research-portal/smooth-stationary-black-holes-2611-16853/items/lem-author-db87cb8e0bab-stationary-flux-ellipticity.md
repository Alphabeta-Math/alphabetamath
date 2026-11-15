---
id: lem-author-db87cb8e0bab-stationary-flux-ellipticity
title: Ellipticity and zero-slope forcing of the stationary maximal flux
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-normal-graph-and-mean-curvature-data
  - math:def-holder-spaces-c-k-alpha-and-their-scaled-norms
  - math:thm-chain-rule-for-total-derivatives
  - math:lem-derivative-algebra-and-chain-rules
  - math:lem-matrix-inversion-preserves-ck-regularity
  - math:cor-determinant-is-a-polynomial-in-the-matrix-entries
  - math:cor-bounded-derivative-implies-lipschitz
  - math:cor-inverse-matrix-by-adjugate
dependency_roles:
  def-normal-graph-and-mean-curvature-data: mathematical-premise
  math:def-holder-spaces-c-k-alpha-and-their-scaled-norms: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:lem-derivative-algebra-and-chain-rules: mathematical-premise
  math:lem-matrix-inversion-preserves-ck-regularity: mathematical-premise
  math:cor-determinant-is-a-polynomial-in-the-matrix-entries: mathematical-premise
  math:cor-bounded-derivative-implies-lipschitz: mathematical-premise
  math:cor-inverse-matrix-by-adjugate: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Fix $0<\alpha<1$, $R_0\ge1$, a bounded annulus $A=\{y\in\mathbb R^3:a<|y|<b\}$ with $0<a<b$, and $p_0>0$. For $R\ge R_0$, let $G_R(y)$ be a smooth symmetric Lorentzian metric matrix of signature $(-,+,+,+)$, independent of the time coordinate. Write $G_R^{\mu\nu}$ for its inverse entries, $J_R=\sqrt{-\det G_R}$, $C_R^{ij}=G_R^{ij}$, $d_R^i=G_R^{i0}$, and $Q_R(y,p)=-G_R^{00}+2d_R^jp_j-C_R^{jk}p_jp_k$, with spatial indices summed from $1$ to $3$. Assume, uniformly in $R$ and on $A\times\{|p|\le p_0\}$, that $Q_R\ge\kappa>0$, $C_R\ge\kappa I$, and $G_R,G_R^{-1},J_R,J_R^{-1}$ have common zeroth-order bounds $M$. Define $P_R^i(y,p)=J_R(C_R^{ij}p_j-d_R^i)/\sqrt{Q_R}$. Then $A_R^{ij}=\partial_{p_j}P_R^i$ is symmetric, with $\lambda I\le A_R\le\Lambda I$ for positive constants depending only on $\kappa,M,p_0$.

If, in addition, $\sup_{R\ge R_0}\|G_R\|_{C^{4,\alpha}(A)}\le M_4$, then $P_R$ has common joint $C^{4,\alpha}$ bounds in $(y,p)$ on this fixed product domain, depending only on $A,\alpha,p_0,\kappa,M,M_4$.

For the zero-slope conclusion, assume $h_R:=J_R/\sqrt{-G_R^{00}}$ has a common $C^{3,\alpha}(A)$ bound $H$ and $\|d_R\|_{C^{3,\alpha}(A)}\le K R^{-2}$. Then, with the $y$ derivatives taken at fixed $p$, $s_R(y,0):=\sum_i\partial_{y_i}P_R^i(y,0)$ satisfies $\|s_R(\cdot,0)\|_{C^{2,\alpha}(A)}\le C H K R^{-2}$, where $C$ depends only on $A,\alpha$. The preceding uniform $C^{4,\alpha}$ hypothesis on $G_R$ supplies the required bound on $h_R$; the zeroth-order hypotheses alone do not.

## Facts & Assumptions

[F1] The Lorentzian and stationary flow-graph conventions are those of the graph definition; maximality means zero mean curvature. This lemma proves analytic properties of the specified flux. Identifying that flux with a particular graph equation is a separate application. [[def-normal-graph-and-mean-curvature-data]]

[F2] Coefficient norms are ordinary Euclidean Hölder norms, applied componentwise; joint norms differentiate in both $y$ and $p$. The parameter $R$ is not a differentiation variable. [[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]]

[F3] For composable totally differentiable Euclidean maps, $D(g\circ f)=Dg(f)Df$. It applies to the smooth coefficient maps here, repeatedly through order four. [[math:thm-chain-rule-for-total-derivatives]]

[F4] Scalar sums, products, quotients with nonzero denominator, compositions and positive integer powers have their usual derivative rules. Apply these rules on coordinate lines and iterate for partial derivatives. [[math:lem-derivative-algebra-and-chain-rules]]

[F5] Matrix inversion preserves every finite $C^k$ class where the determinant is nonzero, and the determinant is a fixed finite polynomial in the matrix entries. [[math:lem-matrix-inversion-preserves-ck-regularity]] [[math:cor-determinant-is-a-polynomial-in-the-matrix-entries]]

[F6] A scalar function on an interval with bounded derivative is Lipschitz with that bound; it applies to restrictions along the piecewise smooth paths used below. [[math:cor-bounded-derivative-implies-lipschitz]]

[F7] For a square matrix over a commutative ring with invertible determinant, $A^{-1}=\det(A)^{-1}\operatorname{adj}(A)$. Apply this to the real $4\times4$ matrices $G_R$, whose determinants are nonzero by the Lorentzian hypothesis. [[math:cor-inverse-matrix-by-adjugate]]

## Proof

**Given:** The hypotheses in the Statement, retaining the additional regularity hypotheses for the corresponding conclusions.

**Goal:** Prove uniform ellipticity, coefficient regularity and the differentiated zero-slope estimate.

1.1 Fix $R$ and put $z_R=C_Rp-d_R$. Symmetry of $C_R$ gives $\partial_{p_j}Q_R=-2z_R^j$. The scalar derivative rules and chain rule give $A_R=J_R(C_R/\sqrt{Q_R}+z_R\otimes z_R/Q_R^{3/2})$. This is symmetric. For every $\xi\in\mathbb R^3$, $\xi^TA_R\xi\ge J_R\kappa|\xi|^2/\sqrt{Q_R}$. The zeroth-order bounds and fixed slope ball bound $Q_R$ above and $z_R$ in norm; also $J_R\ge M^{-1}$ and $Q_R\ge\kappa$. Thus this lower bound is uniform and positive, and the displayed formula gives a uniform upper bound. [given, F3, F4, algebra]

1.2 Assume the additional $C^{4,\alpha}$ bound on $G_R$. By [F5], inversion is smooth on the invertible locus and determinant is polynomial. The identities $\sqrt{t+u}-\sqrt t=u/(\sqrt{t+u}+\sqrt t)$ and $(\sqrt t)'=1/(2\sqrt t)$, together with [F4], give all higher derivatives of $t^{1/2}$ and $t^{-1/2}$ for $t>0$. Their derivatives of any fixed order are bounded when $t$ is bounded away from zero and above. The bound on $J_R^{-1}$ gives $-\det G_R\ge M^{-2}$. The cofactor-over-determinant formula in [F7] expresses every derivative of inversion in the matrix entries as a polynomial numerator divided by a power of the determinant. Bounded matrix entries and this determinant lower bound therefore give common bounds on these derivatives, also on a fixed neighborhood of the matrix values; polynomial increment estimates keep the determinant away from zero on that neighborhood. Repeated use of [F3] and [F4], and $Q_R\ge\kappa$, expresses every mixed derivative of $P_R$ through order four as a finite sum of bounded coefficient functions times derivatives of $G_R$ of order at most four and bounded slope monomials. This proves the required derivative supremum bounds. [given, F3, F4, F5, F7, algebra]

2.1 For scalar factors, $a(x)b(x)-a(x')b(x')=a(x)(b(x)-b(x'))+b(x')(a(x)-a(x'))$ gives $[ab]_\alpha\le\|a\|_\infty[b]_\alpha+\|b\|_\infty[a]_\alpha$. The same identity iterates over finite products. Lower-order derivatives of $G_R$ are uniformly Lipschitz on $A$: two points can be joined by a radial segment and a shorter circular arc at the smaller radius, of total length at most $(1+\pi/2)$ times their Euclidean distance; use [F3] and [F6] on these path pieces with the next-derivative bound. On the product domain the slope points can additionally be joined by a straight segment. Thus these lower derivatives have common Hölder bounds on the bounded domain. The smooth coefficient functions from step 1.2 are uniformly Lipschitz as functions of the bounded matrix entries and slopes: their derivatives are bounded on a common neighborhood, so nearby pairs use a straight segment and [F6], while separated pairs use their supremum bounds. Applying the product inequality to the differentiated expressions in step 1.2, using the assumed Hölder bound on fourth derivatives of $G_R$, proves the joint $C^{4,\alpha}$ bound. The identical argument through order three at $p=0$, where $-G_R^{00}=Q_R(y,0)\ge\kappa$, bounds $h_R$ uniformly under the additional metric hypothesis. [given, F2, F3, F4, F6, step 1.2, algebra]

3.1 For the zero-slope estimate use its explicit $C^{3,\alpha}$ hypotheses on $h_R,d_R$, whether supplied directly or obtained for $h_R$ in step 2.1. Since $P_R(y,0)=-h_Rd_R$, one has $s_R(y,0)=-\sum_i((\partial_i h_R)d_R^i+h_R\partial_i d_R^i)$. Differentiating this formula at most twice gives only finite products of derivatives of $h_R$ and $d_R$ of order at most three. The lower-order Hölder control and product inequality of step 2.1 yield $\|s_R(\cdot,0)\|_{C^{2,\alpha}(A)}\le C\|h_R\|_{C^{3,\alpha}(A)}\|d_R\|_{C^{3,\alpha}(A)}\le C H K R^{-2}$. All constants are independent of $R$. The graph terminology in [F1] imposes no additional equation in this analytic proof. [given, F1, F2, F4, F6, step 2.1, algebra] ∎
