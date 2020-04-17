The Littlewood-Paley Theory and Multipliers
===========================================

In this book notation, the Fourier transform of <img src="https://www.zhihu.com/equation?tex=f" alt="f" class="ee_img tr_noresize" eeimg="1"> is
<img src="https://www.zhihu.com/equation?tex=\int f(x)e^{2\pi i t\cdot x} dx" alt="\int f(x)e^{2\pi i t\cdot x} dx" class="ee_img tr_noresize" eeimg="1"> instead of
<img src="https://www.zhihu.com/equation?tex=\int f(x)e^{-2\pi i t\cdot x} dx" alt="\int f(x)e^{-2\pi i t\cdot x} dx" class="ee_img tr_noresize" eeimg="1">. And the inverse Fourier transform in
this book is <img src="https://www.zhihu.com/equation?tex=\int \hat{f}(x)e^{-2\pi i t\cdot x} dx" alt="\int \hat{f}(x)e^{-2\pi i t\cdot x} dx" class="ee_img tr_noresize" eeimg="1">. But we will still
use the common notation.

There are three main topic originally in the Littlewood-Paley theory:

1.  The auxiliary <img src="https://www.zhihu.com/equation?tex=g" alt="g" class="ee_img tr_noresize" eeimg="1">-function

2.  Partial sum operators and the dyadic decomposition

3.  Marcinkiewicz multiplier theorem

All these three topics are related to multipliers. The auxiliary
<img src="https://www.zhihu.com/equation?tex=g" alt="g" class="ee_img tr_noresize" eeimg="1">-function helps us prove Mihlin multiplier theorem (section 3) and
further some multipliers in <img src="https://www.zhihu.com/equation?tex=M_p" alt="M_p" class="ee_img tr_noresize" eeimg="1"> for specific <img src="https://www.zhihu.com/equation?tex=p" alt="p" class="ee_img tr_noresize" eeimg="1">. Partial sum operator
(section 4) shows some indicate functions of convex sets are
multipliers. Also with help of partial sum operator, we can prove
Marcinkiewicz multiplier theorem (section 6). This theorem and Mihlin
multiplier theorem overlap and neither includes the other.

The first tool: The Littlewood-Paley <img src="https://www.zhihu.com/equation?tex=g" alt="g" class="ee_img tr_noresize" eeimg="1">-function
-------------------------------------------------

For a function <img src="https://www.zhihu.com/equation?tex=f\in L^p(\mathbb{R}^n)" alt="f\in L^p(\mathbb{R}^n)" class="ee_img tr_noresize" eeimg="1">, we define its Poisson integral
is: 
<img src="https://www.zhihu.com/equation?tex=u(x,y)=\int_{\mathbb{R}^n}P_y(t)f(x-t)d t\\" alt="u(x,y)=\int_{\mathbb{R}^n}P_y(t)f(x-t)d t\\" class="ee_img tr_noresize" eeimg="1">

 where
<img src="https://www.zhihu.com/equation?tex=P_y(t)=\int_{\mathbb{R}^n}e^{-2\pi\left\lvert x\right\rvert y}e^{-2\pi i t\cdot x }dx=\frac{c_ny}{(\left\lvert t\right\rvert^2+y^2)^{\frac{n+1}{2}}}" alt="P_y(t)=\int_{\mathbb{R}^n}e^{-2\pi\left\lvert x\right\rvert y}e^{-2\pi i t\cdot x }dx=\frac{c_ny}{(\left\lvert t\right\rvert^2+y^2)^{\frac{n+1}{2}}}" class="ee_img tr_noresize" eeimg="1">.
The <img src="https://www.zhihu.com/equation?tex=g" alt="g" class="ee_img tr_noresize" eeimg="1">-function of <img src="https://www.zhihu.com/equation?tex=f" alt="f" class="ee_img tr_noresize" eeimg="1"> is:

<img src="https://www.zhihu.com/equation?tex=g(f)(x)=\left( \int_{0}^{\infty} \left\lvert\nabla u(x,y)\right\rvert^2 y d y\right)^\frac{1}{2}\\" alt="g(f)(x)=\left( \int_{0}^{\infty} \left\lvert\nabla u(x,y)\right\rvert^2 y d y\right)^\frac{1}{2}\\" class="ee_img tr_noresize" eeimg="1">


One application of <img src="https://www.zhihu.com/equation?tex=g" alt="g" class="ee_img tr_noresize" eeimg="1">-function is it can control the norm of <img src="https://www.zhihu.com/equation?tex=f" alt="f" class="ee_img tr_noresize" eeimg="1">:

[\[thm: g-function control f\]]{#thm: g-function control f
label="thm: g-function control f"} Suppose <img src="https://www.zhihu.com/equation?tex=f\in L^p(\mathbb{R}^n)" alt="f\in L^p(\mathbb{R}^n)" class="ee_img tr_noresize" eeimg="1">,
<img src="https://www.zhihu.com/equation?tex=1<p<\infty" alt="1<p<\infty" class="ee_img tr_noresize" eeimg="1">. Then <img src="https://www.zhihu.com/equation?tex=g(f)\in L^p(\mathbb{R}^n)" alt="g(f)\in L^p(\mathbb{R}^n)" class="ee_img tr_noresize" eeimg="1"> and

<img src="https://www.zhihu.com/equation?tex=A'_p\lVert f\rVert_p\leq \lVert g(f)\rVert_p\leq A_p\lVert f\rVert_p\\" alt="A'_p\lVert f\rVert_p\leq \lVert g(f)\rVert_p\leq A_p\lVert f\rVert_p\\" class="ee_img tr_noresize" eeimg="1">



For <img src="https://www.zhihu.com/equation?tex=p=2" alt="p=2" class="ee_img tr_noresize" eeimg="1">, we have identity
<img src="https://www.zhihu.com/equation?tex=\lVert g(f)\rVert_2= 2^{-\frac{1}{2}}\lVert f\rVert_2" alt="\lVert g(f)\rVert_2= 2^{-\frac{1}{2}}\lVert f\rVert_2" class="ee_img tr_noresize" eeimg="1">. This identity
is important in dyadic decomposition.

The part <img src="https://www.zhihu.com/equation?tex=\lVert g(f)\rVert_p\leq A_p\lVert f\rVert_p" alt="\lVert g(f)\rVert_p\leq A_p\lVert f\rVert_p" class="ee_img tr_noresize" eeimg="1"> is from
vector-valued analogues of singular integral.

Define

<img src="https://www.zhihu.com/equation?tex=\mathscr{H}_2^0=\left\{ f: \left\lvert f\right\rvert^2=\int_{0}^{\infty}\left\lvert f(y)\right\rvert^2y dy<\infty \right\}\\" alt="\mathscr{H}_2^0=\left\{ f: \left\lvert f\right\rvert^2=\int_{0}^{\infty}\left\lvert f(y)\right\rvert^2y dy<\infty \right\}\\" class="ee_img tr_noresize" eeimg="1">


and <img src="https://www.zhihu.com/equation?tex=\mathscr{H}_2" alt="\mathscr{H}_2" class="ee_img tr_noresize" eeimg="1"> be the direct sum of n+1 copies of
<img src="https://www.zhihu.com/equation?tex=\mathscr{H}_2^0" alt="\mathscr{H}_2^0" class="ee_img tr_noresize" eeimg="1">.

The kernel of singular integral here is
<img src="https://www.zhihu.com/equation?tex=K_\epsilon(x)=(\frac{\partial P_{y+\epsilon(x)}}{\partial y},\frac{\partial P_{y+\epsilon(x)}}{\partial x_1},\dots,\frac{\partial P_{y+\epsilon(x)}}{\partial x_k})" alt="K_\epsilon(x)=(\frac{\partial P_{y+\epsilon(x)}}{\partial y},\frac{\partial P_{y+\epsilon(x)}}{\partial x_1},\dots,\frac{\partial P_{y+\epsilon(x)}}{\partial x_k})" class="ee_img tr_noresize" eeimg="1">.
Notice
<img src="https://www.zhihu.com/equation?tex=\left\lvert\nabla u(x,y+\epsilon)\right\rvert^2\leq \left\lvert\nabla u(x,y)\right\rvert^2" alt="\left\lvert\nabla u(x,y+\epsilon)\right\rvert^2\leq \left\lvert\nabla u(x,y)\right\rvert^2" class="ee_img tr_noresize" eeimg="1">.
We have
<img src="https://www.zhihu.com/equation?tex=\left\lvert T_\epsilon(f)(x)\right\rvert=\left\lvert\int_{\mathbb{R}^n}{K_\epsilon(t)f(x-t)dt}\right\rvert\leq g(f)(x)" alt="\left\lvert T_\epsilon(f)(x)\right\rvert=\left\lvert\int_{\mathbb{R}^n}{K_\epsilon(t)f(x-t)dt}\right\rvert\leq g(f)(x)" class="ee_img tr_noresize" eeimg="1">
(<img src="https://www.zhihu.com/equation?tex=T_\epsilon(f)(x)" alt="T_\epsilon(f)(x)" class="ee_img tr_noresize" eeimg="1"> is in Hilbert space) and <img src="https://www.zhihu.com/equation?tex=T_\epsilon(f)(x)" alt="T_\epsilon(f)(x)" class="ee_img tr_noresize" eeimg="1">
converges to <img src="https://www.zhihu.com/equation?tex=g(f)(x)" alt="g(f)(x)" class="ee_img tr_noresize" eeimg="1"> pointwise.

The converse part <img src="https://www.zhihu.com/equation?tex=A'_p\lVert f\rVert_p\leq \lVert g(f)\rVert_p" alt="A'_p\lVert f\rVert_p\leq \lVert g(f)\rVert_p" class="ee_img tr_noresize" eeimg="1"> is by
polarization to the identity, Holder inequality and dual of <img src="https://www.zhihu.com/equation?tex=L^p" alt="L^p" class="ee_img tr_noresize" eeimg="1">.

The function <img src="https://www.zhihu.com/equation?tex=g_{\lambda}^*" alt="g_{\lambda}^*" class="ee_img tr_noresize" eeimg="1">
----------------------------

First section is relied on singular integral. In this section we give
the same result based on characteristic properties of harmonic
functions. The ideas here are useful when singular integral is not
applicable.

Author shows how to avoid singular integral method to prove the
following inequality 
<img src="https://www.zhihu.com/equation?tex=\label{ieq: first control}
    \lVert g(f)\rVert_p\leq A_p\lVert f\rVert_p\quad (1<p\leq 2)\\" alt="\label{ieq: first control}
    \lVert g(f)\rVert_p\leq A_p\lVert f\rVert_p\quad (1<p\leq 2)\\" class="ee_img tr_noresize" eeimg="1">

 The
case <img src="https://www.zhihu.com/equation?tex=2<p<\infty" alt="2<p<\infty" class="ee_img tr_noresize" eeimg="1"> is not shown here.

In the rest of this section, we talk about the positive function
<img src="https://www.zhihu.com/equation?tex=g_{\lambda}^*" alt="g_{\lambda}^*" class="ee_img tr_noresize" eeimg="1">

<img src="https://www.zhihu.com/equation?tex=(g_{\lambda}^*(f)(x))^2=\int_{0}^{\infty}\int_{t\in \mathbb{R}^n}{(\frac{y}{\left\lvert t\right\rvert+y})^{\lambda n}\left\lvert\nabla u(x-t,y)\right\rvert^2 y^{1-n}dt dy}\\" alt="(g_{\lambda}^*(f)(x))^2=\int_{0}^{\infty}\int_{t\in \mathbb{R}^n}{(\frac{y}{\left\lvert t\right\rvert+y})^{\lambda n}\left\lvert\nabla u(x-t,y)\right\rvert^2 y^{1-n}dt dy}\\" class="ee_img tr_noresize" eeimg="1">


The first important inequality is:

<img src="https://www.zhihu.com/equation?tex=g(f)(x)\leq CS(f)(x)\leq C_\lambda g_{\lambda}^*(f)(x)\\" alt="g(f)(x)\leq CS(f)(x)\leq C_\lambda g_{\lambda}^*(f)(x)\\" class="ee_img tr_noresize" eeimg="1">

 where

<img src="https://www.zhihu.com/equation?tex=(S(f)(x))^2=\int_{\Gamma(x)}{\left\lvert\nabla u(t,y)\right\rvert^2 y^{1-n}dydt}=\int_{\Gamma}{\left\lvert\nabla u(x-t,y)\right\rvert^2 y^{1-n}dydt}\\" alt="(S(f)(x))^2=\int_{\Gamma(x)}{\left\lvert\nabla u(t,y)\right\rvert^2 y^{1-n}dydt}=\int_{\Gamma}{\left\lvert\nabla u(x-t,y)\right\rvert^2 y^{1-n}dydt}\\" class="ee_img tr_noresize" eeimg="1">


where
<img src="https://www.zhihu.com/equation?tex=\Gamma=\left\{ (t,y)\in \mathbb{R}_+^{n+1}: \left\lvert t\right\rvert<y, y>0\right\}" alt="\Gamma=\left\{ (t,y)\in \mathbb{R}_+^{n+1}: \left\lvert t\right\rvert<y, y>0\right\}" class="ee_img tr_noresize" eeimg="1">
and <img src="https://www.zhihu.com/equation?tex=\Gamma(x)" alt="\Gamma(x)" class="ee_img tr_noresize" eeimg="1"> is cone <img src="https://www.zhihu.com/equation?tex=\Gamma" alt="\Gamma" class="ee_img tr_noresize" eeimg="1"> with vertex at <img src="https://www.zhihu.com/equation?tex=x" alt="x" class="ee_img tr_noresize" eeimg="1">.

The second important inequality is:

<img src="https://www.zhihu.com/equation?tex=\lVert g_{\lambda}^*(f)(x)\rVert_p\leq A_{p,\lambda}\lVert f\rVert_p\quad (1<p<\infty, p>\frac{2}{\lambda}).\\" alt="\lVert g_{\lambda}^*(f)(x)\rVert_p\leq A_{p,\lambda}\lVert f\rVert_p\quad (1<p<\infty, p>\frac{2}{\lambda}).\\" class="ee_img tr_noresize" eeimg="1">



The case <img src="https://www.zhihu.com/equation?tex=p\geq 2" alt="p\geq 2" class="ee_img tr_noresize" eeimg="1"> is by proving
<img src="https://www.zhihu.com/equation?tex=\lVert g_{\lambda}^*(f)\rVert_p\leq A_\lambda\lVert g(f)\rVert_p" alt="\lVert g_{\lambda}^*(f)\rVert_p\leq A_\lambda\lVert g(f)\rVert_p" class="ee_img tr_noresize" eeimg="1"> and
inequality
[\[ieq: first control\]](#ieq: first control){reference-type="eqref"
reference="ieq: first control"}. It is interesting that the p-norm of
<img src="https://www.zhihu.com/equation?tex=g(f)" alt="g(f)" class="ee_img tr_noresize" eeimg="1">, <img src="https://www.zhihu.com/equation?tex=g_{\lambda}^*(f)" alt="g_{\lambda}^*(f)" class="ee_img tr_noresize" eeimg="1"> can control each other when <img src="https://www.zhihu.com/equation?tex=p\geq 2" alt="p\geq 2" class="ee_img tr_noresize" eeimg="1">.

The proof for the case <img src="https://www.zhihu.com/equation?tex=p<2" alt="p<2" class="ee_img tr_noresize" eeimg="1"> is like the proof for inequality
[\[ieq: first control\]](#ieq: first control){reference-type="eqref"
reference="ieq: first control"}.

We conclude that the norm of <img src="https://www.zhihu.com/equation?tex=g_{\lambda}^*(f)" alt="g_{\lambda}^*(f)" class="ee_img tr_noresize" eeimg="1">, <img src="https://www.zhihu.com/equation?tex=g(f)" alt="g(f)" class="ee_img tr_noresize" eeimg="1">, <img src="https://www.zhihu.com/equation?tex=S(f)" alt="S(f)" class="ee_img tr_noresize" eeimg="1">, <img src="https://www.zhihu.com/equation?tex=f" alt="f" class="ee_img tr_noresize" eeimg="1"> can
control each other.

Multipliers (first version)
---------------------------

Most of results in this section can be found in section 6, chapter 2 in
Rubio's *Weighted Norm inequalities and Related topics*. And proofs of
results are in my note of that book.

Multiplier <img src="https://www.zhihu.com/equation?tex=m" alt="m" class="ee_img tr_noresize" eeimg="1"> is related to a linear transformation <img src="https://www.zhihu.com/equation?tex=T_m" alt="T_m" class="ee_img tr_noresize" eeimg="1"> defined as:

<img src="https://www.zhihu.com/equation?tex=(T_mf)^\wedge(x)=m(x)\hat{f}(x)\\" alt="(T_mf)^\wedge(x)=m(x)\hat{f}(x)\\" class="ee_img tr_noresize" eeimg="1">

 and we shall say that <img src="https://www.zhihu.com/equation?tex=m" alt="m" class="ee_img tr_noresize" eeimg="1"> is a
multiplier for <img src="https://www.zhihu.com/equation?tex=L^p" alt="L^p" class="ee_img tr_noresize" eeimg="1"> if: 
<img src="https://www.zhihu.com/equation?tex=\lVert T_mf\rVert_p\leq \lVert f\rVert_p\\" alt="\lVert T_mf\rVert_p\leq \lVert f\rVert_p\\" class="ee_img tr_noresize" eeimg="1">



Multipliers has some general properties:

1.  <img src="https://www.zhihu.com/equation?tex=M_p" alt="M_p" class="ee_img tr_noresize" eeimg="1"> is a Banach algebra under pointwise multiplication.

2.  <img src="https://www.zhihu.com/equation?tex=M_2" alt="M_2" class="ee_img tr_noresize" eeimg="1"> is identical with the bounded measurable function <img src="https://www.zhihu.com/equation?tex=L^\infty" alt="L^\infty" class="ee_img tr_noresize" eeimg="1">.

3.  <img src="https://www.zhihu.com/equation?tex=M_1" alt="M_1" class="ee_img tr_noresize" eeimg="1"> is identical with the finite Borel measures <img src="https://www.zhihu.com/equation?tex=\mathscr{B}" alt="\mathscr{B}" class="ee_img tr_noresize" eeimg="1">
    (Refer Theorem 2.5.8 in *Classical Fourier Analysis*).

4.  Suppose <img src="https://www.zhihu.com/equation?tex=\frac{1}{p}+\frac{1}{q}=1" alt="\frac{1}{p}+\frac{1}{q}=1" class="ee_img tr_noresize" eeimg="1">, <img src="https://www.zhihu.com/equation?tex=1\leq p,q\leq \infty" alt="1\leq p,q\leq \infty" class="ee_img tr_noresize" eeimg="1">, then
    <img src="https://www.zhihu.com/equation?tex=M_p=M_q" alt="M_p=M_q" class="ee_img tr_noresize" eeimg="1"> with identity of norms.

5.  <img src="https://www.zhihu.com/equation?tex=M_\infty" alt="M_\infty" class="ee_img tr_noresize" eeimg="1"> is identical with the finite Borel measures <img src="https://www.zhihu.com/equation?tex=\mathscr{B}" alt="\mathscr{B}" class="ee_img tr_noresize" eeimg="1">
    (By 3 and 4).

Then we prove two important multiplier theorems. The first is Mihlin
multiplier theorem:

Suppose that <img src="https://www.zhihu.com/equation?tex=m(x)" alt="m(x)" class="ee_img tr_noresize" eeimg="1"> is of class <img src="https://www.zhihu.com/equation?tex=C^k" alt="C^k" class="ee_img tr_noresize" eeimg="1"> in the complement of the origin of
<img src="https://www.zhihu.com/equation?tex=\mathbb{R}^n" alt="\mathbb{R}^n" class="ee_img tr_noresize" eeimg="1">, where <img src="https://www.zhihu.com/equation?tex=k" alt="k" class="ee_img tr_noresize" eeimg="1"> is an integer greater than <img src="https://www.zhihu.com/equation?tex=\frac{n}{2}" alt="\frac{n}{2}" class="ee_img tr_noresize" eeimg="1">.
Assume also that for every differential monomial
<img src="https://www.zhihu.com/equation?tex=(\frac{\partial}{\partial x})^\alpha" alt="(\frac{\partial}{\partial x})^\alpha" class="ee_img tr_noresize" eeimg="1">,
<img src="https://www.zhihu.com/equation?tex=\alpha=(\alpha_1,\alpha_2,\dots,\alpha_n)" alt="\alpha=(\alpha_1,\alpha_2,\dots,\alpha_n)" class="ee_img tr_noresize" eeimg="1">, with
<img src="https://www.zhihu.com/equation?tex=\left\lvert\alpha\right\rvert=\alpha_1+\alpha_2+\cdots+\alpha_n" alt="\left\lvert\alpha\right\rvert=\alpha_1+\alpha_2+\cdots+\alpha_n" class="ee_img tr_noresize" eeimg="1">, we
have: 
<img src="https://www.zhihu.com/equation?tex=\label{ieq: Mihlin}
        \left\lvert\frac{\partial}{\partial x}^\alpha m(x)\right\rvert\leq B\left\lvert x\right\rvert^{-\left\lvert\alpha\right\rvert},\quad \left\lvert\alpha\right\rvert\leq k\\" alt="\label{ieq: Mihlin}
        \left\lvert\frac{\partial}{\partial x}^\alpha m(x)\right\rvert\leq B\left\lvert x\right\rvert^{-\left\lvert\alpha\right\rvert},\quad \left\lvert\alpha\right\rvert\leq k\\" class="ee_img tr_noresize" eeimg="1">


Then <img src="https://www.zhihu.com/equation?tex=m\in M_p" alt="m\in M_p" class="ee_img tr_noresize" eeimg="1">, <img src="https://www.zhihu.com/equation?tex=1<p<\infty" alt="1<p<\infty" class="ee_img tr_noresize" eeimg="1">

And the second is Hörmander Mihlin multiplier theorem:

The assumption [\[ieq: Mihlin\]](#ieq: Mihlin){reference-type="eqref"
reference="ieq: Mihlin"} can be replaced by the weaker assumptions:

<img src="https://www.zhihu.com/equation?tex=\left\lvert m(x)\right\rvert\leq B\\" alt="\left\lvert m(x)\right\rvert\leq B\\" class="ee_img tr_noresize" eeimg="1">



<img src="https://www.zhihu.com/equation?tex=\sup_{0<R<\infty}R^{2\left\lvert\alpha\right\rvert+n}\int_{R\leq\left\lvert x\right\rvert\leq 2R}{\left\lvert\frac{\partial}{\partial x}^\alpha m(x)\right\rvert^2 dx}\leq B,\quad \left\lvert\alpha\right\rvert\leq k\\" alt="\sup_{0<R<\infty}R^{2\left\lvert\alpha\right\rvert+n}\int_{R\leq\left\lvert x\right\rvert\leq 2R}{\left\lvert\frac{\partial}{\partial x}^\alpha m(x)\right\rvert^2 dx}\leq B,\quad \left\lvert\alpha\right\rvert\leq k\\" class="ee_img tr_noresize" eeimg="1">



The proof of Mihlin multiplier theorem can be done with help of
g-functions and their variants:

Under the assumption
[\[ieq: Mihlin\]](#ieq: Mihlin){reference-type="eqref"
reference="ieq: Mihlin"}, let us set for each <img src="https://www.zhihu.com/equation?tex=f\in L^2" alt="f\in L^2" class="ee_img tr_noresize" eeimg="1">:

<img src="https://www.zhihu.com/equation?tex=F(x)=(T_mf)(x)\\" alt="F(x)=(T_mf)(x)\\" class="ee_img tr_noresize" eeimg="1">

 Then

<img src="https://www.zhihu.com/equation?tex=g_1(F,x)\leq B_\lambda g_\lambda^*(f,x),\quad \lambda=\frac{2k}{n}\\" alt="g_1(F,x)\leq B_\lambda g_\lambda^*(f,x),\quad \lambda=\frac{2k}{n}\\" class="ee_img tr_noresize" eeimg="1">



By above lemma, we have:

<img src="https://www.zhihu.com/equation?tex=\lVert T_mf\rVert_p=\lVert F\rVert_p\leq A_1\lVert g_1(F,x)\rVert_p\leq A_2\lVert g_\lambda^*(f,x)\rVert_p\leq A_3\lVert f\rVert_p\\" alt="\lVert T_mf\rVert_p=\lVert F\rVert_p\leq A_1\lVert g_1(F,x)\rVert_p\leq A_2\lVert g_\lambda^*(f,x)\rVert_p\leq A_3\lVert f\rVert_p\\" class="ee_img tr_noresize" eeimg="1">


I can not understand the proof of corollary in the end of this section.

The second tool: partial sums operators
---------------------------------------

Given a rectangle <img src="https://www.zhihu.com/equation?tex=\rho" alt="\rho" class="ee_img tr_noresize" eeimg="1">, we define he partial sum operator <img src="https://www.zhihu.com/equation?tex=S_\rho(f)" alt="S_\rho(f)" class="ee_img tr_noresize" eeimg="1">
to be: 
<img src="https://www.zhihu.com/equation?tex=S_\rho(f)^\wedge=\chi_\rho\hat{f}\\" alt="S_\rho(f)^\wedge=\chi_\rho\hat{f}\\" class="ee_img tr_noresize" eeimg="1">

 and for this operator we
have: 
<img src="https://www.zhihu.com/equation?tex=\label{ieq: partial sum operator inequality}
    \lVert S_\rho(f)\rVert_p\leq A_p\lVert f\rVert_p\quad 1<p<\infty\\" alt="\label{ieq: partial sum operator inequality}
    \lVert S_\rho(f)\rVert_p\leq A_p\lVert f\rVert_p\quad 1<p<\infty\\" class="ee_img tr_noresize" eeimg="1">


This bounded linear operator has an extended version on function space
<img src="https://www.zhihu.com/equation?tex=L^p(\mathbb{R}^n,\mathscr{H})" alt="L^p(\mathbb{R}^n,\mathscr{H})" class="ee_img tr_noresize" eeimg="1">, where <img src="https://www.zhihu.com/equation?tex=\mathscr{H}" alt="\mathscr{H}" class="ee_img tr_noresize" eeimg="1"> is the sequence
Hilbert space:
<img src="https://www.zhihu.com/equation?tex=\mathscr{H}=\{(c_j)_{j=1}^\infty:(\sum_j\left\lvert c_j\right\rvert^2)^\frac{1}{2}< \infty\}" alt="\mathscr{H}=\{(c_j)_{j=1}^\infty:(\sum_j\left\lvert c_j\right\rvert^2)^\frac{1}{2}< \infty\}" class="ee_img tr_noresize" eeimg="1">.

Given a sequence of rectangle <img src="https://www.zhihu.com/equation?tex=\mathscr{R}=\{\rho_j\}_{j=1}^\infty" alt="\mathscr{R}=\{\rho_j\}_{j=1}^\infty" class="ee_img tr_noresize" eeimg="1">, we
define

<img src="https://www.zhihu.com/equation?tex=S_{\mathscr{R}}(f)=(S_{\rho_1}(f_1),\dots,S_{\rho_j}(f_j),\dots)\\" alt="S_{\mathscr{R}}(f)=(S_{\rho_1}(f_1),\dots,S_{\rho_j}(f_j),\dots)\\" class="ee_img tr_noresize" eeimg="1">


where 
<img src="https://www.zhihu.com/equation?tex=f=(f_1,\dots,f_j,\dots)\\" alt="f=(f_1,\dots,f_j,\dots)\\" class="ee_img tr_noresize" eeimg="1">



The general version of inequality
[\[ieq: partial sum operator inequality\]](#ieq: partial sum operator inequality){reference-type="eqref"
reference="ieq: partial sum operator inequality"} is

<img src="https://www.zhihu.com/equation?tex=\label{ieq: partial sum operator inequality 2}
    \lVert S_{\mathscr{R}}(f)\rVert_p\leq A_p\lVert f\rVert_p\quad 1<p<\infty\\" alt="\label{ieq: partial sum operator inequality 2}
    \lVert S_{\mathscr{R}}(f)\rVert_p\leq A_p\lVert f\rVert_p\quad 1<p<\infty\\" class="ee_img tr_noresize" eeimg="1">



To prove this theorem, we use vector-valued analogues of Hilbert
transform. But first we consider the one dimensional and single valued
case. We have following identity for operator <img src="https://www.zhihu.com/equation?tex=S_{(-\infty,0)}" alt="S_{(-\infty,0)}" class="ee_img tr_noresize" eeimg="1">:

<img src="https://www.zhihu.com/equation?tex=\label{eq: Hilbert for -infty to 0}
    S_{(-\infty,0)}=\frac{I+iH}{2}\\" alt="\label{eq: Hilbert for -infty to 0}
    S_{(-\infty,0)}=\frac{I+iH}{2}\\" class="ee_img tr_noresize" eeimg="1">

 For one dimensional and
vector-valued case, by property of vector-valued singular integral, we
have: 
<img src="https://www.zhihu.com/equation?tex=\lVert\tilde{H}f\rVert_p\leq A_p\lVert f\rVert_p\\" alt="\lVert\tilde{H}f\rVert_p\leq A_p\lVert f\rVert_p\\" class="ee_img tr_noresize" eeimg="1">

 where
<img src="https://www.zhihu.com/equation?tex=\tilde{H}f=(Hf_1,\dots,Hf_j,\dots)" alt="\tilde{H}f=(Hf_1,\dots,Hf_j,\dots)" class="ee_img tr_noresize" eeimg="1">. Combining with equation
[\[eq: Hilbert for -infty to 0\]](#eq: Hilbert for -infty to 0){reference-type="eqref"
reference="eq: Hilbert for -infty to 0"}, we have inequality
[\[ieq: partial sum operator inequality 2\]](#ieq: partial sum operator inequality 2){reference-type="eqref"
reference="ieq: partial sum operator inequality 2"} holds when <img src="https://www.zhihu.com/equation?tex=f" alt="f" class="ee_img tr_noresize" eeimg="1"> is
vector-valued with single variable and <img src="https://www.zhihu.com/equation?tex=\mathscr{R}" alt="\mathscr{R}" class="ee_img tr_noresize" eeimg="1"> is collection of
rectangles <img src="https://www.zhihu.com/equation?tex=(-\infty,0)" alt="(-\infty,0)" class="ee_img tr_noresize" eeimg="1">.

By translation, we can show:

<img src="https://www.zhihu.com/equation?tex=S_{(-\infty,a_j)}f_j(x)=\frac{f_j+ie^{2\pi i x\cdot a_j}H(e^{-2\pi i x\cdot a_j}f_j)}{2}\\" alt="S_{(-\infty,a_j)}f_j(x)=\frac{f_j+ie^{2\pi i x\cdot a_j}H(e^{-2\pi i x\cdot a_j}f_j)}{2}\\" class="ee_img tr_noresize" eeimg="1">


Thus inequality
[\[ieq: partial sum operator inequality 2\]](#ieq: partial sum operator inequality 2){reference-type="eqref"
reference="ieq: partial sum operator inequality 2"} holds when <img src="https://www.zhihu.com/equation?tex=f" alt="f" class="ee_img tr_noresize" eeimg="1"> is
vector-valued with single variable and <img src="https://www.zhihu.com/equation?tex=\mathscr{R}" alt="\mathscr{R}" class="ee_img tr_noresize" eeimg="1"> is collection of
rectangles <img src="https://www.zhihu.com/equation?tex=(-\infty,a_j)" alt="(-\infty,a_j)" class="ee_img tr_noresize" eeimg="1">.

To prove n dimensional case, we claim:

The linear span of form <img src="https://www.zhihu.com/equation?tex=f'(x_1)f''(x_2,\dots,x_n)" alt="f'(x_1)f''(x_2,\dots,x_n)" class="ee_img tr_noresize" eeimg="1"> is dense in
<img src="https://www.zhihu.com/equation?tex=L^2(\mathbb{R}^n)" alt="L^2(\mathbb{R}^n)" class="ee_img tr_noresize" eeimg="1">.

This lemma is true since we can choose <img src="https://www.zhihu.com/equation?tex=f'" alt="f'" class="ee_img tr_noresize" eeimg="1"> and <img src="https://www.zhihu.com/equation?tex=f''" alt="f''" class="ee_img tr_noresize" eeimg="1"> as orthogonal
basis of <img src="https://www.zhihu.com/equation?tex=L^2(\mathbb{R})" alt="L^2(\mathbb{R})" class="ee_img tr_noresize" eeimg="1"> and <img src="https://www.zhihu.com/equation?tex=L^2(\mathbb{R}^{n-1})" alt="L^2(\mathbb{R}^{n-1})" class="ee_img tr_noresize" eeimg="1">. By this lemma,
we can consider first variable <img src="https://www.zhihu.com/equation?tex=x_1" alt="x_1" class="ee_img tr_noresize" eeimg="1"> separately. Thus inequality
[\[ieq: partial sum operator inequality 2\]](#ieq: partial sum operator inequality 2){reference-type="eqref"
reference="ieq: partial sum operator inequality 2"} holds when <img src="https://www.zhihu.com/equation?tex=f" alt="f" class="ee_img tr_noresize" eeimg="1"> is
vector-valued with n variables and <img src="https://www.zhihu.com/equation?tex=\mathscr{R}" alt="\mathscr{R}" class="ee_img tr_noresize" eeimg="1"> is collection of half
space <img src="https://www.zhihu.com/equation?tex=\{x:x_1<a_j\}_{j=1}^\infty" alt="\{x:x_1<a_j\}_{j=1}^\infty" class="ee_img tr_noresize" eeimg="1">.

Finally since finite rectangle is the intersection of 2n half-spaces, a
2n-fold of previous result proves the inequality
[\[ieq: partial sum operator inequality 2\]](#ieq: partial sum operator inequality 2){reference-type="eqref"
reference="ieq: partial sum operator inequality 2"} where <img src="https://www.zhihu.com/equation?tex=\mathscr{R}" alt="\mathscr{R}" class="ee_img tr_noresize" eeimg="1">
contains finite rectangles. The result is not depended on number of
rectangles. Thus using limit argument the inequality
[\[ieq: partial sum operator inequality 2\]](#ieq: partial sum operator inequality 2){reference-type="eqref"
reference="ieq: partial sum operator inequality 2"} holds for infinite
number of rectangles.

The author describes two problems:

1.  Let <img src="https://www.zhihu.com/equation?tex=B" alt="B" class="ee_img tr_noresize" eeimg="1"> be the unit ball in <img src="https://www.zhihu.com/equation?tex=\mathbb{R}^n" alt="\mathbb{R}^n" class="ee_img tr_noresize" eeimg="1">. Can we replace the
    rectangle <img src="https://www.zhihu.com/equation?tex=\rho" alt="\rho" class="ee_img tr_noresize" eeimg="1"> by the ball <img src="https://www.zhihu.com/equation?tex=B" alt="B" class="ee_img tr_noresize" eeimg="1"> in inequality
    [\[ieq: partial sum operator inequality\]](#ieq: partial sum operator inequality){reference-type="eqref"
    reference="ieq: partial sum operator inequality"}?.

2.  Can the rectangles of inequality
    [\[ieq: partial sum operator inequality 2\]](#ieq: partial sum operator inequality 2){reference-type="eqref"
    reference="ieq: partial sum operator inequality 2"} be replaced by
    rectangles that are each arbitrarily rotated?

We know the the answer of first problems can be affirmative only in the
range <img src="https://www.zhihu.com/equation?tex=\frac{2n}{n+1}<p<\frac{2n}{n-1}" alt="\frac{2n}{n+1}<p<\frac{2n}{n-1}" class="ee_img tr_noresize" eeimg="1">. The solution of first problem
implies the resolution of the second problem for the same <img src="https://www.zhihu.com/equation?tex=p" alt="p" class="ee_img tr_noresize" eeimg="1">. And the
answer of the second problem is in the negative for <img src="https://www.zhihu.com/equation?tex=p" alt="p" class="ee_img tr_noresize" eeimg="1"> outside the
interval <img src="https://www.zhihu.com/equation?tex=\frac{2n}{n+1}\leq p\leq \frac{2n}{n-1}" alt="\frac{2n}{n+1}\leq p\leq \frac{2n}{n-1}" class="ee_img tr_noresize" eeimg="1">.

Also there is a continuous analogue of inequality
[\[ieq: partial sum operator inequality 2\]](#ieq: partial sum operator inequality 2){reference-type="eqref"
reference="ieq: partial sum operator inequality 2"}. Let
<img src="https://www.zhihu.com/equation?tex=(\Gamma,d\gamma)" alt="(\Gamma,d\gamma)" class="ee_img tr_noresize" eeimg="1"> be an abstract measure space. We can replace the
sequence Hilbert space by square integrable functions space
<img src="https://www.zhihu.com/equation?tex=L^2(\Gamma,d\gamma)" alt="L^2(\Gamma,d\gamma)" class="ee_img tr_noresize" eeimg="1">. And <img src="https://www.zhihu.com/equation?tex=\rho_\gamma=\rho(\gamma)" alt="\rho_\gamma=\rho(\gamma)" class="ee_img tr_noresize" eeimg="1"> is a measurable
function from <img src="https://www.zhihu.com/equation?tex=\Gamma" alt="\Gamma" class="ee_img tr_noresize" eeimg="1"> to rectangles in <img src="https://www.zhihu.com/equation?tex=\mathbb{R}^n" alt="\mathbb{R}^n" class="ee_img tr_noresize" eeimg="1">.

The dyadic decomposition
------------------------

First we introduce the dyadic decomposition of <img src="https://www.zhihu.com/equation?tex=\mathbb{R}" alt="\mathbb{R}" class="ee_img tr_noresize" eeimg="1">. We
decompose <img src="https://www.zhihu.com/equation?tex=\mathbb{R}\setminus \{0\}" alt="\mathbb{R}\setminus \{0\}" class="ee_img tr_noresize" eeimg="1"> as
<img src="https://www.zhihu.com/equation?tex=(\cup_{k=\infty}^\infty [2^k,2^{k+1}])\cup(\cup_{k=\infty}^\infty [-2^{k+1},-2^k])" alt="(\cup_{k=\infty}^\infty [2^k,2^{k+1}])\cup(\cup_{k=\infty}^\infty [-2^{k+1},-2^k])" class="ee_img tr_noresize" eeimg="1">.
Then we consider the product of intervals in decomposition of
<img src="https://www.zhihu.com/equation?tex=\mathbb{R}" alt="\mathbb{R}" class="ee_img tr_noresize" eeimg="1">. This is the dyadic decomposition of <img src="https://www.zhihu.com/equation?tex=\mathbb{R}^n" alt="\mathbb{R}^n" class="ee_img tr_noresize" eeimg="1"> and we
denote as <img src="https://www.zhihu.com/equation?tex=\Delta" alt="\Delta" class="ee_img tr_noresize" eeimg="1">.

Recall the partial sum operator, we have:

<img src="https://www.zhihu.com/equation?tex=\sum_{\rho\in \Delta}S_{\rho}=I\\" alt="\sum_{\rho\in \Delta}S_{\rho}=I\\" class="ee_img tr_noresize" eeimg="1">

 and since the rectangles in
decomposition are disjoint, by Plancherel's theorem we have:

<img src="https://www.zhihu.com/equation?tex=\label{eq: decomposition 2-norm}
    \sum_{\rho\in \Delta}\lVert S_{\rho}f\rVert_2^2=\lVert f\rVert_2^2\\" alt="\label{eq: decomposition 2-norm}
    \sum_{\rho\in \Delta}\lVert S_{\rho}f\rVert_2^2=\lVert f\rVert_2^2\\" class="ee_img tr_noresize" eeimg="1">


The special property of partial sum operator on dyadic decomposition is
we can control the norm of <img src="https://www.zhihu.com/equation?tex=f" alt="f" class="ee_img tr_noresize" eeimg="1"> by this partial sum operator:

[\[thm: dyadic decomposition\]]{#thm: dyadic decomposition
label="thm: dyadic decomposition"} Suppose <img src="https://www.zhihu.com/equation?tex=f\in L^p" alt="f\in L^p" class="ee_img tr_noresize" eeimg="1">, <img src="https://www.zhihu.com/equation?tex=1<p<\infty" alt="1<p<\infty" class="ee_img tr_noresize" eeimg="1">.
Then
<img src="https://www.zhihu.com/equation?tex=\left( \sum_{\rho\in \Delta}\left\lvert S_{\rho}f(x)\right\rvert^2 \right)^\frac{1}{2}\in L^p" alt="\left( \sum_{\rho\in \Delta}\left\lvert S_{\rho}f(x)\right\rvert^2 \right)^\frac{1}{2}\in L^p" class="ee_img tr_noresize" eeimg="1">
and

<img src="https://www.zhihu.com/equation?tex=A_p\lVert f\rVert_p\leq \lVert( \sum_{\rho\in \Delta}\left\lvert S_{\rho}f(x)\right\rvert^2)^\frac{1}{2}\rVert_p\leq B_p\lVert f\rVert_p\\" alt="A_p\lVert f\rVert_p\leq \lVert( \sum_{\rho\in \Delta}\left\lvert S_{\rho}f(x)\right\rvert^2)^\frac{1}{2}\rVert_p\leq B_p\lVert f\rVert_p\\" class="ee_img tr_noresize" eeimg="1">



To prove above theorem we need Rademacher functions <img src="https://www.zhihu.com/equation?tex=\{r_i(t)\}_{i=1}" alt="\{r_i(t)\}_{i=1}" class="ee_img tr_noresize" eeimg="1">
on integral <img src="https://www.zhihu.com/equation?tex=(0,1)" alt="(0,1)" class="ee_img tr_noresize" eeimg="1">. <img src="https://www.zhihu.com/equation?tex=r_0(t)" alt="r_0(t)" class="ee_img tr_noresize" eeimg="1"> is defined to be: 
<img src="https://www.zhihu.com/equation?tex=r_0(t)=
    \left\{\begin{aligned}
        1\quad 0<t\leq \frac{1}{2}\\
        -1\quad \frac{1}{2}\leq t< 1
    \end{aligned}\right.\\" alt="r_0(t)=
    \left\{\begin{aligned}
        1\quad 0<t\leq \frac{1}{2}\\
        -1\quad \frac{1}{2}\leq t< 1
    \end{aligned}\right.\\" class="ee_img tr_noresize" eeimg="1">

 and <img src="https://www.zhihu.com/equation?tex=r_m(t)" alt="r_m(t)" class="ee_img tr_noresize" eeimg="1"> is defined to be <img src="https://www.zhihu.com/equation?tex=r_0(2^mt)" alt="r_0(2^mt)" class="ee_img tr_noresize" eeimg="1"> and
they are extended outside by periodicity. The important of Rademacher
functions is all p-norms of linear combination of Rademacher functions
are comparable:

Suppose <img src="https://www.zhihu.com/equation?tex=\sum\left\lvert a_m\right\rvert^2<\infty" alt="\sum\left\lvert a_m\right\rvert^2<\infty" class="ee_img tr_noresize" eeimg="1"> and set
<img src="https://www.zhihu.com/equation?tex=F(t)=\sum a_mr_m(t)" alt="F(t)=\sum a_mr_m(t)" class="ee_img tr_noresize" eeimg="1">. Then <img src="https://www.zhihu.com/equation?tex=F(t)\in L^p" alt="F(t)\in L^p" class="ee_img tr_noresize" eeimg="1"> for all <img src="https://www.zhihu.com/equation?tex=p<\infty" alt="p<\infty" class="ee_img tr_noresize" eeimg="1"> and

<img src="https://www.zhihu.com/equation?tex=A_p\lVert F\rVert_p\leq\lVert F\rVert_2=\left( \sum_{m=0}^\infty\left\lvert a_m\right\rvert^2 \right)^{\frac{1}{2}}\leq B_p\lVert F\rVert_p\\" alt="A_p\lVert F\rVert_p\leq\lVert F\rVert_2=\left( \sum_{m=0}^\infty\left\lvert a_m\right\rvert^2 \right)^{\frac{1}{2}}\leq B_p\lVert F\rVert_p\\" class="ee_img tr_noresize" eeimg="1">



By equation
[\[eq: decomposition 2-norm\]](#eq: decomposition 2-norm){reference-type="eqref"
reference="eq: decomposition 2-norm"}, we only need to proof one
inequality in theorem
[\[thm: dyadic decomposition\]](#thm: dyadic decomposition){reference-type="ref"
reference="thm: dyadic decomposition"}:

<img src="https://www.zhihu.com/equation?tex=\lVert( \sum_{\rho\in \Delta}\left\lvert S_{\rho}f(x)\right\rvert^2)^\frac{1}{2}\rVert_p\leq B_p\lVert f\rVert_p\\" alt="\lVert( \sum_{\rho\in \Delta}\left\lvert S_{\rho}f(x)\right\rvert^2)^\frac{1}{2}\rVert_p\leq B_p\lVert f\rVert_p\\" class="ee_img tr_noresize" eeimg="1">


The other inequality is by polarization and dual of <img src="https://www.zhihu.com/equation?tex=L^p" alt="L^p" class="ee_img tr_noresize" eeimg="1">.

The Marcinkiewicz multiplier theorem
------------------------------------

The Marcinkiewicz multiplier theorem is one of the most important
results of the Littlewood-Paley theory

Let <img src="https://www.zhihu.com/equation?tex=m" alt="m" class="ee_img tr_noresize" eeimg="1"> be a bounded function on <img src="https://www.zhihu.com/equation?tex=\mathbb{R}^n" alt="\mathbb{R}^n" class="ee_img tr_noresize" eeimg="1"> of the type described.
Suppose also

1.  <img src="https://www.zhihu.com/equation?tex=\left\lvert m\right\rvert\leq B" alt="\left\lvert m\right\rvert\leq B" class="ee_img tr_noresize" eeimg="1">

2.  for each <img src="https://www.zhihu.com/equation?tex=0<k\leq n" alt="0<k\leq n" class="ee_img tr_noresize" eeimg="1">
    
<img src="https://www.zhihu.com/equation?tex=\sup_{x_{k+1},\dots,x_n}\int_{\rho}\left\lvert\frac{\partial^km}{\partial x_1\dots\partial x_k}\right\rvert dx_1\dots dx_k\leq B\\" alt="\sup_{x_{k+1},\dots,x_n}\int_{\rho}\left\lvert\frac{\partial^km}{\partial x_1\dots\partial x_k}\right\rvert dx_1\dots dx_k\leq B\\" class="ee_img tr_noresize" eeimg="1">



3.  The condition analogous to 2. is valid for every on of the <img src="https://www.zhihu.com/equation?tex=n!" alt="n!" class="ee_img tr_noresize" eeimg="1">
    permutations of the variables <img src="https://www.zhihu.com/equation?tex=x_1,\dots,x_n" alt="x_1,\dots,x_n" class="ee_img tr_noresize" eeimg="1">.

Then <img src="https://www.zhihu.com/equation?tex=m\in M_p" alt="m\in M_p" class="ee_img tr_noresize" eeimg="1">, <img src="https://www.zhihu.com/equation?tex=1<p<\infty" alt="1<p<\infty" class="ee_img tr_noresize" eeimg="1">; and more precisely, if
<img src="https://www.zhihu.com/equation?tex=f\in L^2\cap L^p" alt="f\in L^2\cap L^p" class="ee_img tr_noresize" eeimg="1">, <img src="https://www.zhihu.com/equation?tex=\lVert T_mf\rVert_p\leq A_p\lVert f\rVert_p" alt="\lVert T_mf\rVert_p\leq A_p\lVert f\rVert_p" class="ee_img tr_noresize" eeimg="1"> where
<img src="https://www.zhihu.com/equation?tex=A_p" alt="A_p" class="ee_img tr_noresize" eeimg="1"> depends only on <img src="https://www.zhihu.com/equation?tex=B" alt="B" class="ee_img tr_noresize" eeimg="1">, <img src="https://www.zhihu.com/equation?tex=p" alt="p" class="ee_img tr_noresize" eeimg="1"> and <img src="https://www.zhihu.com/equation?tex=n" alt="n" class="ee_img tr_noresize" eeimg="1">.

The difference between Hörmander multiplier theorem and Marcinkiewicz
multiplier theorem can be illustrated by invariance considerations. The
class of multipliers in Hömander multiplier theorem is invariant under
dilations, <img src="https://www.zhihu.com/equation?tex=m(x)\mapsto m(\epsilon x)" alt="m(x)\mapsto m(\epsilon x)" class="ee_img tr_noresize" eeimg="1"> and rotations
<img src="https://www.zhihu.com/equation?tex=m(x)\mapsto m(\rho^{-1} x)" alt="m(x)\mapsto m(\rho^{-1} x)" class="ee_img tr_noresize" eeimg="1">. But the class of multipliers in
Marcinkiewicz multiplier theorem is invariant under a larger group of
dilations, <img src="https://www.zhihu.com/equation?tex=m(x)\mapsto m(\epsilon\circ x)" alt="m(x)\mapsto m(\epsilon\circ x)" class="ee_img tr_noresize" eeimg="1">, where
<img src="https://www.zhihu.com/equation?tex=\epsilon\circ x=(\epsilon_1x_1,\dots,\epsilon_nx_n)" alt="\epsilon\circ x=(\epsilon_1x_1,\dots,\epsilon_nx_n)" class="ee_img tr_noresize" eeimg="1">. But it not
invariant under rotations.

Let <img src="https://www.zhihu.com/equation?tex=\Delta" alt="\Delta" class="ee_img tr_noresize" eeimg="1"> denote the dyadic decomposition and <img src="https://www.zhihu.com/equation?tex=f\in L^2\cap L^p" alt="f\in L^2\cap L^p" class="ee_img tr_noresize" eeimg="1">, and
write <img src="https://www.zhihu.com/equation?tex=F=T_mf" alt="F=T_mf" class="ee_img tr_noresize" eeimg="1">. To prove this theorem, we only need to show:

<img src="https://www.zhihu.com/equation?tex=\lVert(\sum_{\rho\in \Delta}\left\lvert S_\rho F\right\rvert^2)^\frac{1}{2}\rVert_p\leq C_p\lVert(\sum_{\rho\in \Delta}\left\lvert S_\rho f\right\rvert^2)^\frac{1}{2}\rVert_p\\" alt="\lVert(\sum_{\rho\in \Delta}\left\lvert S_\rho F\right\rvert^2)^\frac{1}{2}\rVert_p\leq C_p\lVert(\sum_{\rho\in \Delta}\left\lvert S_\rho f\right\rvert^2)^\frac{1}{2}\rVert_p\\" class="ee_img tr_noresize" eeimg="1">


Using Theorem
[\[thm: dyadic decomposition\]](#thm: dyadic decomposition){reference-type="ref"
reference="thm: dyadic decomposition"} we conclude <img src="https://www.zhihu.com/equation?tex=m\in M_p" alt="m\in M_p" class="ee_img tr_noresize" eeimg="1">.
