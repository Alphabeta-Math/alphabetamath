---
title: A specified future ingoing Kerr extension and its time orientation
status: draft
research_item: def-author-cea8e61dc3c6-kerr-ingoing-extension
dependency_level: 2
sources:
  references:
    - title: The Kerr Metric
      url: https://arxiv.org/pdf/1410.2130
      locator: §2, equations (2.1), (2.5)–(2.8), PDF pp. 2–3
      statement: The review gives ingoing and Boyer–Lindquist Kerr forms, their
        coordinate transformation, and the asymptotic identification of mass M
        and angular momentum J=aM.
      hypotheses: The Kerr metric in the stated coordinate systems and their indicated
        domains.
      reading_limits: Consulted the cited formulas and adjacent discussion in section
        2, PDF pages 2–3. These provide coordinate background only; the
        parameter-independent sphere construction, embedding, signature and
        time-orientation calculations are supplied locally below. No source
        proof of the full indexed statement was reconstructed.
---

## Prerequisites

- [lem-author-cea8e61dc3c6-kerr-exterior-tensor](item-lem-author-cea8e61dc3c6-kerr-exterior-tensor)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [physics:def-emg-xs-kn-data](https://alphabetamath.cc/physics/item/def-emg-xs-kn-data)
- [math:ex-the-n-sphere-with-its-standard-smooth-atlas](https://alphabetamath.cc/item/ex-the-n-sphere-with-its-standard-smooth-atlas)
- [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)
- [` The Kerr Metric · §2, equations (2.1), (2.5)–(2.8), PDF pp. 2–3 `](https://arxiv.org/pdf/1410.2130)


## Definition

Fix $M>0$, $|a|\leq M$ and $r_\pm=M\pm\sqrt{M^2-a^2}$ as in the exterior tensor. The future ingoing Kerr extension used here is $\mathcal K^{\mathrm{in}}=\mathbb R_v\times(0,\infty)_r\times S^2$, with $\Sigma=r^2+a^2\cos^2\theta$, $\Delta=r^2-2Mr+a^2$ and metric
$$g=-(1-2Mr/\Sigma)dv^2+2dv\,dr-4Mar\sin^2\theta\,dv\,d\psi/\Sigma-2a\sin^2\theta\,dr\,d\psi+\Sigma\,d\theta^2+(r^2+a^2+2Ma^2r\sin^2\theta/\Sigma)\sin^2\theta\,d\psi^2.$$
Here $\psi$ has period $2\pi$. Precisely, take $S^2=\{(x,y,z)\in\mathbb R^3:x^2+y^2+z^2=1\}$ with its standard smooth atlas and inclusion $\iota:S^2\to\mathbb R^3$. Define the round metric $\gamma=\iota^*(dx^2+dy^2+dz^2)$, the tangent rotation field $\xi(x,y,z)=(-y,x,0)$, and its metric-dual one-form $\alpha=\gamma(\xi,\cdot)=\iota^*(x\,dy-y\,dx)$. On a polar chart $(x,y,z)=(\sin\theta\cos\psi,\sin\theta\sin\psi,\cos\theta)$, these are $\gamma=d\theta^2+\sin^2\theta\,d\psi^2$ and $\alpha=\sin^2\theta\,d\psi$. Globally, the displayed metric means the following tensor, with the sphere tensors pulled back to the product and $\Sigma=r^2+a^2z^2$:
$$g=-(1-2Mr/\Sigma)dv^2+2dv\,dr-(4Mar/\Sigma)dv\,\alpha-2a\,dr\,\alpha+\Sigma\gamma+a^2(1+2Mr/\Sigma)\alpha^2.$$
Products in these line elements denote symmetric tensor products, with $\beta\omega=(\beta\otimes\omega+\omega\otimes\beta)/2$. This sphere construction does not restrict $a$ to the subextremal range.

Put $\tau=v-r$ and choose $-\nabla\tau$ to be future timelike, using the inverse-metric and time-orientation conventions for stationary Lorentzian data. The exterior embeds by $v=t+F(r)$ and $\psi=\phi+G(r)$ with $F'=(r^2+a^2)/\Delta$ and $G'=a/\Delta$; additive constants merely choose origins. On the sphere this angular map is the rotation $R_{G(r)}$, where $R_\lambda(x,y,z)=(x\cos\lambda-y\sin\lambda,x\sin\lambda+y\cos\lambda,z)$. The exterior coordinate tensor used for the substitution is the uncharged case $q=0$, $x^0=t$ of the Boyer–Lindquist formula, restricted to $r>r_+$ and $0<\theta<\pi$; its global exterior smoothness and signature are those of the exterior tensor. This specifies a global future extension with one selected exterior. It does not assert that this patch is the maximal analytic extension or contains a bifurcation sphere.

## Definition references

[lem-author-cea8e61dc3c6-kerr-exterior-tensor](item-lem-author-cea8e61dc3c6-kerr-exterior-tensor)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[physics:def-emg-xs-kn-data](https://alphabetamath.cc/physics/item/def-emg-xs-kn-data)

[math:ex-the-n-sphere-with-its-standard-smooth-atlas](https://alphabetamath.cc/item/ex-the-n-sphere-with-its-standard-smooth-atlas)

[math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)

## Facts & Assumptions

[F1] The exterior supplier fixes $M>0$, $|a|\leq M$, $r_\pm$, the smooth Lorentzian exterior tensor on $r>r_+$, and $\Delta>0$, $\Sigma>0$ there, including the extremal range. [lem-author-cea8e61dc3c6-kerr-exterior-tensor](item-lem-author-cea8e61dc3c6-kerr-exterior-tensor)

[F2] The inverse metric, metric dual and future-direction conventions are those of the stationary Lorentzian data. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F3] The coordinate supplier defines $g=-\Delta(dx^0-a\sin^2\theta\,d\phi)^2/\Sigma+\Sigma\,dr^2/\Delta+\Sigma\,d\theta^2+\sin^2\theta((r^2+a^2)d\phi-a\,dx^0)^2/\Sigma$ on $\Sigma>0$, $\Delta\ne0$, $0<\theta<\pi$, with $\Delta=r^2-2Mr+a^2+q^2$. Here use only $q=0$, $x^0=t$, $r>r_+$; no axis or horizon extension is imported from this supplier. [physics:def-emg-xs-kn-data](https://alphabetamath.cc/physics/item/def-emg-xs-kn-data)

[F4] The standard sphere supplier with $n=2$ supplies the unit sphere and its smooth stereographic atlas. The pullback supplier defines restriction of ambient covariant tensors along the smooth inclusion and pullback of the sphere tensors to the product. The rotation field, round metric and rotation one-form used here are the explicit local constructions in the Definition. [math:ex-the-n-sphere-with-its-standard-smooth-atlas](https://alphabetamath.cc/item/ex-the-n-sphere-with-its-standard-smooth-atlas) [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)

## Justification

**Given:** The parameters and global tensor in the Definition, with the exterior properties [F1], tensor and orientation conventions [F2], pole-free coordinate formula [F3], and sphere and pullback interfaces [F4].

**Goal:** Justify smoothness, signature, embedding and time orientation.

1.1 The sphere inclusion is smooth in the stereographic atlas of [F4], as its inverse chart formulas have smooth rational ambient components. Its induced Euclidean metric $\gamma$ is smooth, and $\xi$ is tangent since $x(-y)+yx+z\cdot0=0$. For any tangent vector $X$, $\gamma(\xi,X)=-y\,dx(X)+x\,dy(X)$, proving the stated formula for the smooth one-form $\alpha$. The polar parametrization yields the displayed expressions for $\gamma$ and $\alpha$. Since $r>0$ gives $\Sigma=r^2+a^2z^2\geq r^2>0$, every coefficient of the global tensor is smooth. Its angular part agrees with the polar metric because $r^2+a^2=\Sigma+a^2\sin^2\theta$, so it is $\Sigma\gamma+a^2(1+2Mr/\Sigma)\alpha^2$. This establishes smoothness at both poles without dividing by $\sin\theta$ or assuming $|a|<M$. [given, F4, algebra]

2.1 On the exterior, [F1] gives $\Delta>0$, so the smooth radial primitives $F,G$ exist on the interval $(r_+,\infty)$. Substitute $dt=dv-(r^2+a^2)dr/\Delta$ and $d\phi=d\psi-a\,dr/\Delta$ in [F3]. Writing $A=r^2+a^2$ and $b=\sin^2\theta$, the two squared forms become $dt-ab\,d\phi=dv-ab\,d\psi-(\Sigma/\Delta)dr$ and $A\,d\phi-a\,dt=A\,d\psi-a\,dv$. Thus the $dr^2$ term cancels and expansion gives exactly the polar metric in the Definition. The global coordinate map is $(t,r,p)\mapsto(t+F(r),r,R_{G(r)}p)$, with smooth inverse $(v,r,p)\mapsto(v-F(r),r,R_{-G(r)}p)$. Rotations are smooth also at the poles, so this is a diffeomorphism onto $r>r_+$ of the extension. Equality of its pulled-back metric with the exterior tensor holds on the dense pole-free region by substitution and hence at the poles by smoothness. [given, F1, F3, F4, step 1.1, algebra]

3.1 The determinant relative to $dv\,dr$ and round-sphere area is $-\Sigma^2$. It is nonzero for every $r>0$, including $r=r_+$ and the poles, so the exterior Lorentzian signature extends throughout this connected product. Direct matrix inversion on the pole-free region gives $g^{vv}=a^2\sin^2\theta/\Sigma$, $g^{vr}=(r^2+a^2)/\Sigma$, $g^{rr}=\Delta/\Sigma$; the resulting scalar identities extend to the poles by smoothness. Hence $g^{-1}(d\tau,d\tau)=-1-2Mr/\Sigma<0$. Thus the chosen time orientation is smooth by [F2]. Near infinity, $T=\partial_t=\partial_v$ is timelike and $g(-\nabla\tau,T)=-d\tau(T)=-1<0$, so it is future-directed. None of these computations divides by $r_+-r_-$, so the extremal case is included. [given, F1, F2, step 1.1, step 2.1, algebra] ∎

## External input

The cited Kerr coordinate formulas provide background for the local calculation in this item.
