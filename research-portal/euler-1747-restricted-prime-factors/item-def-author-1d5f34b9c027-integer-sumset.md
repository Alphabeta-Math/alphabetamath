---
title: Sumset of two sets of integers
status: draft
research_item: def-author-1d5f34b9c027-integer-sumset
dependency_level: 0
---

## Prerequisites

- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)


## Definition

Let $S$ and $T$ be subsets of the set $\mathbb Z$ of integers. Their **sumset** is the set of integers obtained by adding one element of $S$ and one element of $T$. Using ordinary integer addition, define

$$S+T=\{n\in\mathbb Z:\text{there exist }s\in S\text{ and }t\in T\text{ with }n=s+t\}.$$

The two choices are independent, so when $S=T$ the same element can be used twice.

## Definition references

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

## Justification

Integer addition assigns a unique integer $s+t$ to each pair of integers $s,t$. The condition that $n$ equals such a sum with $s\in S$ and $t\in T$ selects a unique subset of $\mathbb Z$, because specifying a condition on the elements of a given set determines exactly one subset with that membership condition.
