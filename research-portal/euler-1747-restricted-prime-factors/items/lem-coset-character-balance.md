---
id: lem-coset-character-balance
kind: lemma
title: Balance of a character on a finite coset orbit
status: published
domain: mathematics
deps:
  - math:def-group
  - math:def-subgroup
  - math:def-coset
  - math:def-group-homomorphism
  - math:lem-units-of-z
  - math:def-injection-surjection-bijection
  - math:def-finite-cardinality
  - math:def-power-set
  - math:cor-cardinality-of-the-power-set
  - math:thm-subset-of-a-finite-set
  - math:def-function
  - math:def-subset-and-proper-subset
formulation_deps:
  - math:def-group
  - math:def-subgroup
  - math:def-coset
  - math:def-group-homomorphism
  - math:lem-units-of-z
  - math:def-finite-cardinality
  - math:def-function
  - math:def-subset-and-proper-subset
argument_deps:
  - math:def-group
  - math:def-subgroup
  - math:def-coset
  - math:def-group-homomorphism
  - math:lem-units-of-z
  - math:def-injection-surjection-bijection
  - math:def-finite-cardinality
  - math:def-power-set
  - math:cor-cardinality-of-the-power-set
  - math:thm-subset-of-a-finite-set
  - math:def-function
  - math:def-subset-and-proper-subset
dependency_roles:
  math:def-group: mathematical-premise
  math:def-subgroup: mathematical-premise
  math:def-coset: mathematical-premise
  math:def-group-homomorphism: mathematical-premise
  math:lem-units-of-z: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-power-set: mathematical-premise
  math:cor-cardinality-of-the-power-set: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:def-function: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-generated
  proof: ai-generated
dependency_level: 0
---

## Statement

Let $G$ be a finite group with identity $e$ and let $H,K\le G$ be subgroups. Let $\chi:G\to\{+1,-1\}$ be a character, meaning a homomorphism into the two signs under multiplication. Assume that $\chi(h)=+1$ for every $h\in H$ and that $\chi$ takes both signs on $K$.

Write $Hg=\{hg:h\in H\}$ for the right coset represented by $g$, and $H\backslash G=\{Hg:g\in G\}$ for the set of right cosets. The right $K$-orbit of $H=He$ is the set $\mathcal O=\{Hk:k\in K\}$ of cosets reached from $H$ by right multiplication by elements of $K$. The sign of $Hg$ is $\chi(g)$, independent of the representative. For either $S=\mathcal O$ or $S=H\backslash G$, let $S_+$ and $S_-$ consist of the cosets in $S$ with signs $+1$ and $-1$, respectively. Then $S_+$ and $S_-$ are finite and $|S_+|=|S_-|$.

## Facts & Assumptions

[F1] A group has an associative multiplication, a two-sided identity $e$, and a two-sided inverse $u^{-1}$ for each element $u$ ([[math:def-group]]).

[F2] A subgroup contains the group identity and is closed under multiplication and taking inverses ([[math:def-subgroup]]).

[F3] The right coset represented by $g$ is the subset $Hg=\{hg:h\in H\}$ of $G$ ([[math:def-coset]]).

[F4] The group of units of the integers under multiplication is $\{+1,-1\}$, with identity $+1$ and each sign its own inverse ([[math:lem-units-of-z]]). A group homomorphism preserves multiplication, so $\chi(uv)=\chi(u)\chi(v)$ for $u,v\in G$ ([[math:def-group-homomorphism]]).

[F5] A map is injective if equal outputs imply equal inputs, surjective if each target value occurs, and bijective if both hold ([[math:def-injection-surjection-bijection]]).

[F6] A set is finite when it admits a bijection with $\{0,\ldots,n-1\}$ for some natural number $n$. Its cardinality is that unique $n$, and a bijection between finite sets gives equal cardinalities ([[math:def-finite-cardinality]], clause (d)).

[F7] The power set $\mathcal P(G)$ is the set of all subsets of $G$ ([[math:def-power-set]]).

[F8] A function from a set to a specified codomain assigns each input exactly one output in that codomain ([[math:def-function]]).

[F9] A set is a subset of another set if every element of the first set belongs to the second ([[math:def-subset-and-proper-subset]]).

[L1] The power set of a finite set is finite ([[math:cor-cardinality-of-the-power-set]]).

[L2] Every subset of a finite set is finite ([[math:thm-subset-of-a-finite-set]]).

## Proof

**Given:** The finite group $G$, its subgroups $H,K$, and the character $\chi$ taking only $+1$ on $H$ and both signs on $K$.

**Goal:** Show that the coset sign is well-defined and that $|S_+|=|S_-|$ for both choices of $S$.

1.1 If $Hg'=Hg$, then $g'=eg'\in Hg'$ because $e\in H$. Thus $g'\in Hg$, so $g'=hg$ for some $h\in H$. It follows that $\chi(g')=\chi(h)\chi(g)=\chi(g)$. Every coset has a representative $g$, and the preceding equality makes the value $\bar\chi(Hg)=\chi(g)$ unique in $\{+1,-1\}$. This defines the coset sign function. [F1, F2, F3, F4, F8, given]

1.2 For $u\in G$, right multiplication gives a map $R_u(Hg)=H(gu)$ on $H\backslash G$. Since $gu\in G$, the output $H(gu)$ is in $H\backslash G$. Indeed, $H(gu)=\{xu:x\in Hg\}$ by associativity, so the output depends only on the coset. One has $R_e(C)=C$ and $R_v(R_u(C))=R_{uv}(C)$ for every coset $C$ and all $u,v\in G$. These are the right action identities. Also $He=H$, and $R_k(H)=Hk$ for $k\in K$, so this action gives exactly the stated orbit. If $k,u\in K$, then $ku\in K$, so $R_u$ sends $\mathcal O$ to itself whenever $u\in K$. [F1, F2, F3, F8]

2.1 Choose $t\in K$ with $\chi(t)=-1$. Since $t^{-1}\in K$, both $R_t$ and $R_{t^{-1}}$ act on each set $S$, and their two compositions are the identity by the right action identities. For $C=Hg$ one has $\bar\chi(R_t(C))=\chi(gt)=\bar\chi(C)\chi(t)$. The products $(+1)(-1)=-1$ and $(-1)(-1)=+1$ show that $R_t$ reverses the sign. [F1, F2, F4, given, step 1.1, step 1.2]

3.1 For each $C\in S_+$, step 1.2 gives a unique value $R_t(C)$ and step 2.1 places it in $S_-$. Hence $f(C)=R_t(C)$ defines a function $f:S_+\to S_-$. If $f(C)=f(C')$, applying $R_{t^{-1}}$ yields $C=C'$, so $f$ is injective. Given $D\in S_-$, set $C=R_{t^{-1}}(D)$. Then $C\in S$ and $R_t(C)=D$. Since $R_t$ reverses signs, $C\in S_+$ and $f(C)=D$. Thus $f$ is surjective and hence bijective. [F5, F8, step 1.2, step 2.1]

4.1 Every member of $S_+$ or $S_-$ is a coset and hence a subset of $G$, so each such member lies in the power set $\mathcal P(G)$. Therefore $S_+$ and $S_-$ are both subsets of $\mathcal P(G)$. Since $G$ is finite, the power set is finite, and both sign classes are finite. The bijection gives $|S_+|=|S_-|$ for both the orbit and the full coset set. [F3, F6, F7, F9, L1, L2, given, step 3.1] ∎
