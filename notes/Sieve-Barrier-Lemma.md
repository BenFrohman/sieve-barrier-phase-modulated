# On the Local Commutation Limits of Phase-Modulated Sieve Operators

Benjamin Frohman  
13 September 2026

**Abstract.** A pointwise operator built from truncated factor counts \(\Omega_R\) at level \(R=N^\theta\), \(\theta<1/2\), cannot separate large twin primes from products of two primes larger than \(R\). Embedding Selberg weights in a contour integral in an auxiliary variable \(z\) commutes: the integral factors as a function of \(n\bmod 42\) and leaves the quadratic weight unchanged. This class of operators does not alter the Maynard–Polymath variational problem and does not yield \(H_1=2\). The established unconditional bound remains \(H_1\le 246\).

---

## 1. Lemma: The Local Sieve Barrier

Let \(N\) be a large parameter, and let \(R=N^\theta\) with a fixed sieve exponent \(\theta<1/2\). Let \(\mathcal{H}=\{0,2\}\) be the admissible 2-tuple. Define the truncated factor count

\[
\Omega_R(n)=\sum_{\substack{p\mid n\\ p\le R}}1.
\]

Let \(\gamma\) be a closed contour encircling \(z=0\), and let

\[
f(z;n)=z^{\Omega_R(n)+\Omega_R(n+2)-2}.
\]

Define the localized phase-modulated operator

\[
t_R(n)=\frac{1}{2\pi i}\oint_\gamma\frac{f(z;n)}{z^{1+\varepsilon(n)}}\,dz,
\]

where \(\varepsilon(n)=(n\bmod 42)/208\). The integers \(42\) and \(208\) are parameters of this operator, not of the Maynard integrals. The barrier below holds for any function of \(n\bmod M\), for any fixed modulus \(M\). For non-integer \(\varepsilon\) the integrand has a branch point at \(0\); whatever value is assigned to the integral depends on \(n\) only through \(\varepsilon(n)\).

### Proof of the Local Barrier

Let \(n\sim N\). Let \(\mathcal{P}\) be the class of pairs in which both \(n\) and \(n+2\) are prime. For \(\theta<1/2\) and \(n\) large one has \(n>R\), hence \(\Omega_R(n)=\Omega_R(n+2)=0\).

Let \(\mathcal{E}\) be the class of pairs in which every prime factor of \(n\) and of \(n+2\) exceeds \(R\). This includes high-magnitude \(E_2\times E_2\) pairs and mixed pairs such as \((p,q^2)\) with \(p,q>R\). Then likewise \(\Omega_R(n)=\Omega_R(n+2)=0\).

The generating function is therefore identical on both classes:

\[
f(z;n)\Big|_{n\in\mathcal{P}}=f(z;n)\Big|_{n\in\mathcal{E}_2}=z^{-2}.
\]

The integrand \(z^{-3-\varepsilon(n)}\) depends on \(n\) only through the residue class \(n\bmod 42\). The operator \(t_R(n)\) cannot separate a twin pair from a high-magnitude \(E_2\) pair in the same class.

Check at \(R=\lfloor 1000^{0.35}\rfloor=11\): \((41,43)\in\mathcal{P}\) and \((167,13^2)\) both have \(\Omega_{11}=0,0\) and both have \(n\equiv 41\pmod{42}\). The same contour returns the same value.

\(\blacksquare\)

---

## 2. Theorem: The Quadratic Commutation Barrier

Let

\[
\Lambda_2(n)=\Biggl(\sum_{d\mid n(n+2)}\lambda_d\Biggr)^2
\]

be a Selberg square weight with \(\lambda_d=0\) for \(d>R=N^\theta\). Embedding these weights in the same contour does not remove the barrier of Lemma 1.

### Proof of Commutation

Set

\[
\mathcal{T}(n)=\frac{1}{2\pi i}\oint_\gamma\Biggl(\sum_{d\mid n(n+2)}\lambda_d\Biggr)^2 z^{-1-\varepsilon(n)}\,dz.
\]

The path \(\gamma\) does not depend on \(d\). The finite sum over divisors commutes with the integral:

\[
\mathcal{T}(n)=\Lambda_2(n)\cdot e(n\bmod 42),\qquad
e(n\bmod 42)=\frac{1}{2\pi i}\oint_\gamma z^{-1-\varepsilon(n)}\,dz.
\]

The factor \(e(n\bmod 42)\) is constant on each residue class modulo \(42\). The weight \(\Lambda_2(n)\) is nonnegative. The product cannot change sign inside a class to cancel \(E_2\) terms that share the class of a twin. Summing \(\mathcal{T}(n)\) over \(n\sim N\) therefore scales each class by a static factor and preserves the classical parity error.

\(\blacksquare\)

---

## 3. Analytical Consequences on Bounded Prime Gaps

Lemma 1 and Theorem 2 show that this local phase framework supplies no additional information to the Maynard–Polymath variational problem. The integrals that actually appear there are real integrals of a test function \(F\) on the simplex

\[
\mathcal{R}_k=\{(x_1,\ldots,x_k):x_i\ge 0,\ \textstyle\sum x_i\le 1\}.
\]

They contain no factor \(z^{-1-\varepsilon}\) and no period-\(42\) phase. Consequently this construction does not reduce the ensemble size required to force a positive weighted count, and it does not deduce \(H_1=2\).

The established unconditional theorem remains

\[
H_1\le 246
\]

(Polymath8b, admissible \(50\)-tuple of that diameter). A preprint of Stadlmann (arXiv:2608.31126v1) announces \(240\); that posting is not used here as the established record. Under Elliott–Halberstam one has \(H_1\le 12\); under a generalized form, \(H_1\le 6\). None of those statements is the twin-prime conjecture.

The local phase operator cannot be used to deduce \(H_1=2\).

---

*This note is offered for self-deposit on Zenodo under CC BY 4.0. A DOI is reserved by the depositor.*

---

## 4. Direction of improvement in \(k\)

Under a stronger level of distribution the Maynard ratio \(\rho(F)>1\) becomes available at a *smaller* ensemble size \(k\), hence at a smaller combinatorial diameter \(H(k)\). The direction of improvement is
\[
k\downarrow \quad\Longrightarrow\quad H(k)\downarrow,
\]
not \(k\uparrow\).

- Bombieri–Vinogradov (\(\theta<1/2\)): first crossing at \(k=50\), bound \(H_1\le H(50)=246\).
- Elliott–Halberstam: crossing at \(k=5\), bound \(H_1\le H(5)=12\).
- Generalized Elliott–Halberstam: crossing at \(k=3\), bound \(H_1\le H(3)=6\).
- Twin-prime conjecture: crossing at \(k=2\), bound \(H_1\le H(2)=2\). Open.

Inflating the tuple to \(k=196\) is the opposite of this direction. \(H(196)\asymp 196\log 196+196\approx 10^3\), a worse two-prime diameter at the same level of distribution. This note does not claim \(H_1\le 208\).
