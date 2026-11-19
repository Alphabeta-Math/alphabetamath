---
id: def-quaternion-right-ideal-and-reduced-norm
kind: definition
title: Quaternion right ideals and their reduced norm
status: draft
domain: mathematics
deps:
  - math:def-linear-basis
  - math:thm-any-two-finite-bases-have-the-same-size
  - def-author-24fda87362bc-hamilton-algebra-and-reduced-norm
  - def-author-24fda87362bc-quaternion-orders-and-lattice-completions
  - def-author-24fda87362bc-local-adic-valuation
  - lem-author-24fda87362bc-quaternion-lattice-norms-and-local-generators
  - math:def-subgroup
  - math:def-left-right-and-two-sided-ideal
formulation_deps:
  - math:def-linear-basis
  - def-author-24fda87362bc-hamilton-algebra-and-reduced-norm
  - def-author-24fda87362bc-quaternion-orders-and-lattice-completions
  - def-author-24fda87362bc-local-adic-valuation
  - lem-author-24fda87362bc-quaternion-lattice-norms-and-local-generators
  - math:def-subgroup
  - math:def-left-right-and-two-sided-ideal
argument_deps:
  - math:def-linear-basis
  - math:thm-any-two-finite-bases-have-the-same-size
  - def-author-24fda87362bc-hamilton-algebra-and-reduced-norm
  - def-author-24fda87362bc-quaternion-orders-and-lattice-completions
  - def-author-24fda87362bc-local-adic-valuation
  - lem-author-24fda87362bc-quaternion-lattice-norms-and-local-generators
  - math:def-subgroup
  - math:def-left-right-and-two-sided-ideal
dependency_roles:
  math:def-linear-basis: mathematical-premise
  math:thm-any-two-finite-bases-have-the-same-size: mathematical-premise
  math:def-left-right-and-two-sided-ideal: mathematical-premise
  def-author-24fda87362bc-hamilton-algebra-and-reduced-norm: mathematical-premise
  def-author-24fda87362bc-quaternion-orders-and-lattice-completions: mathematical-premise
  def-author-24fda87362bc-local-adic-valuation: mathematical-premise
  lem-author-24fda87362bc-quaternion-lattice-norms-and-local-generators: mathematical-premise
  math:def-subgroup: mathematical-premise
provenance:
  statement: ai-generated
  proof: not-applicable
dependency_level: 3
---

## Definition

Let $O$ be an order in the rational Hamilton algebra $B$, so $O$ is a unital subring and a full integral lattice. A right fractional $O$-ideal is a full integral lattice $I\subseteq B$ with $io\in I$ for every $i\in I$ and $o\in O$. It is integral if $I\subseteq O$, and principal if $I=xO=\{xo:o\in O\}$ for some $x\in B^\times$, where $B^\times$ denotes the elements with a two-sided inverse. A right ideal of the ring $O$ is an additive subgroup of $O$ stable under this right multiplication by $O$. Every integral right fractional ideal is a right ideal in this sense.

For a prime $\ell$ let $I_\ell$ and $O_\ell$ be the $\mathbb Z_\ell$-spans of $I$ and $O$ in $B_\ell=B(\mathbb Q_\ell)$. A right fractional $O_\ell$-ideal is the $\mathbb Z_\ell$-span of a $\mathbb Q_\ell$-basis of $B_\ell$, with the span required to be stable under right multiplication by $O_\ell$. It is integral if it is contained in $O_\ell$ and principal if it is $x_\ell O_\ell$ for some $x_\ell\in B_\ell^\times$. The fractional ideal $I$ is locally principal if $I_\ell$ is principal at every prime $\ell$.

The reduced norm ideal $\operatorname{nrd}(I)\subseteq\mathbb Q$ is the set of finite $\mathbb Z$-linear combinations of the reduced norms $N(y)$ for $y\in I$. A fractional ideal of $\mathbb Z$ here means a nonzero additive subgroup of $\mathbb Q$ closed under multiplication by integers and contained in $D^{-1}\mathbb Z$ for some positive integer $D$. The positive generator $d$ of $\operatorname{nrd}(I)=d\mathbb Z$ is also called the reduced norm of $I$. For a local right fractional ideal $J$, its reduced norm ideal is the $\mathbb Z_\ell$-span of the reduced norms of elements of $J$. It is of the form $a\mathbb Z_\ell$ for $a\in\mathbb Q_\ell^\times$, and its valuation is $v_\ell(a)$ with $v_\ell(\ell)=1$. The corresponding local norm ideal of $I_\ell$ equals $d\mathbb Z_\ell$. If $J=x_\ell O_\ell$ with $x_\ell$ invertible, its norm ideal is $N(x_\ell)\mathbb Z_\ell$ and has valuation $v_\ell(N(x_\ell))$. If $I=xO$ with $x$ invertible, its positive norm is $N(x)$. Integral ideals have positive integer norm.

## Justification

The full lattices and their completions are those of [[def-author-24fda87362bc-quaternion-orders-and-lattice-completions]]. Expressing a basis of $I$ in a basis of $O$ and clearing the finitely many rational denominators gives a positive integer $D$ with $DI\subseteq O$, as required for fractional scaling. As an integer span, $I$ contains $0$ and is closed under addition and additive inverses. For $I\subseteq O$, it is an additive subgroup of $O$ by [[math:def-subgroup]]. The assumed stability under right multiplication by $O$ gives the remaining condition of [[math:def-left-right-and-two-sided-ideal|the right-ideal definition]]. Multiplication in the Hamilton algebra of [[def-author-24fda87362bc-hamilton-algebra-and-reduced-norm]] is bilinear. Expanding products of local coefficient combinations of basis vectors shows $I_\ell O_\ell\subseteq I_\ell$. If $I=xO$ then the local span is $xO_\ell$ because each rational left multiplication by $x$ extends by the same coordinate rule.

Apply [[lem-author-24fda87362bc-quaternion-lattice-norms-and-local-generators]] to $L=I$. The lemma gives $\operatorname{nrd}(I)=d\mathbb Z$ with $d>0$. This set contains $0$ and is closed under addition and additive inverses, so it is an additive subgroup of $\mathbb Q$ by [[math:def-subgroup]]. It contains the nonzero element $d$, is stable under integer multiplication, and lies in $E^{-1}\mathbb Z$ for a positive integer $E$ clearing the denominator of $d$. Hence it is a fractional ideal of $\mathbb Z$. The same lemma identifies the local span with $d\mathbb Z_\ell$ and computes it for $I_\ell=x_\ell O_\ell$.

For a general $J$, take a $\mathbb Q_\ell$-basis whose $\mathbb Z_\ell$-span is $J$. This basis is a linearly independent spanning set by [[math:def-linear-basis]]. The standard Hamilton basis $1,i,j,k$ has four elements. Hence the basis for $J$ is finite and has four elements by [[math:thm-any-two-finite-bases-have-the-same-size]]. Label them $b_1,\ldots,b_4$. For $t_i\in\mathbb Z_\ell$, expand the four coordinate squares of $\sum_i t_i b_i$ to obtain
$$N(\textstyle\sum_i t_i b_i)=\sum_i t_i^2 N(b_i)+\sum_{i<j}t_i t_j\bigl(N(b_i+b_j)-N(b_i)-N(b_j)\bigr).$$
Thus the norms of the basis vectors and their pairwise sums generate the local norm span. Each of these vectors belongs to the local span of the basis, so its norm is among the generators in the definition. Write $1=\sum_i c_i b_i$ with $c_i\in\mathbb Q_\ell$. Choose a nonnegative integer $n$ such that $n+v_\ell(c_i)\ge0$ for each nonzero $c_i$. By the valuation product law and $v_\ell(\ell)=1$, every $\ell^n c_i$ belongs to $\mathbb Z_\ell$. Thus $\ell^n1$ lies in $J$ and has nonzero norm $\ell^{2n}$. At least one listed norm is nonzero, since otherwise their span could not contain $\ell^{2n}$. By [[def-author-24fda87362bc-local-adic-valuation]], the valuations of these nonzero norms are totally ordered integers. Start with any nonzero listed norm. Compare it with the other nonzero norms in turn, replacing the current norm whenever the next one has smaller valuation. After each comparison the current norm has valuation at most those considered so far. The list is finite, so the last retained norm $a$ has least valuation. For any nonzero generator $s$ in the list, $v_\ell(s/a)=v_\ell(s)-v_\ell(a)\ge0$, so $s\in a\mathbb Z_\ell$. The zero generators also lie in $a\mathbb Z_\ell$. Thus $a$ generates the local span. For $J=x_\ell O_\ell$, the norms of elements of $O_\ell$ lie in $\mathbb Z_\ell$ by the lemma, and include $1$. The equality $N(x_\ell)N(x_\ell^{-1})=N(1)=1$ makes $N(x_\ell)$ nonzero. All norms from $J$ are multiples of $N(x_\ell)$ over $\mathbb Z_\ell$, and taking $1\in O_\ell$ gives the norm $N(x_\ell)$ itself. Any two nonzero scalars generating a local scalar ideal differ by a unit of $\mathbb Z_\ell$, since both ratios between the scalars lie in $\mathbb Z_\ell$. They have equal valuation by [[def-author-24fda87362bc-local-adic-valuation]]. Thus a choice of quaternion generator does not affect the norm valuation. If $I=xO$, the lemma gives $d=N(x)$ since the rational reduced norm of an invertible element is positive. If $I\subseteq O$, each generating norm belongs to $\mathbb Z$ by the same lemma, so $d$ is a positive integer.
