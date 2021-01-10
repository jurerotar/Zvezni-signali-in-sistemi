# Formule Zvezni signali in sistemi

## Frekvenca
$c = \lambda f$

$f = 2 \pi \omega$

## Fourierjeva vrsta
$\omega = \frac{2 \pi }{T}$

$a_0 = \frac{1}{T} \int_{\tau}^{\tau + T} f(x) dx$

### Trigonometrična vrsta

$a_n = \frac{2}{T} \int_{\tau}^{\tau + T} f(t) \cdot cos(\omega n t) dt$

$b_n = \frac{2}{T} \int_{\tau}^{\tau + T} f(t) \cdot sin(\omega n t) dt$

$u(t)= a_0 + \sum_{n = 1}^\infty (a_n \cdot cos(\omega n t) + b_n \cdot sin(\omega n t))$

$c_0 = a_0$

$c_n = \sqrt{a_n^2 + b_n^2}$

$\rho_n = arctg(\frac{b_n}{a_n})$

#### Zveze

$cos(n \pi) = (-1)^n$

$cos(2 n \pi) = 1$

$sin(n \pi)=0$

#### Primeri
$\int x \cdot cos(ax) dx = \frac{x sin(ax)}{a} + \frac{cos(ax)}{a^2}$

$\int x \cdot sin(ax) dx = -\frac{x cos(ax)}{a} + \frac{sin(ax)}{a^2}$

### Eksponenta vrsta

$A_n=\frac{1}{T} \int_{0}^T f(x) \cdot e^{-jn \pi x} dx$

$x(t)=a_0 + \sum_{n \neq 0} A_n$

#### Zveze

$e^{-j \pi n}=(-1)^n$

#### Primeri
$\int e^{ax} dx = \frac{e^{ax}}{a}$

$\int x \cdot e^{ax} dx = \frac{x e^{ax}}{a} - \frac{e^{ax}}{a^2}$



## Teorem o maksimalnem prenosu moči
$Z_b = Z_g^*$

## Resonančna frekvenca
$Im(Z) = 0 \Omega$

## Kvaliteta
$Q = \frac{X_L ( \omega)}{R(\omega)}$

$Q = -\frac{X_C ( \omega)}{R(\omega)}$

## Energijska formula
$Q = \omega \frac{\sum W_C(\omega)}{\sum P(\omega)}$

$W = \int_{0}^T u(t) \cdot i(t) dt$

## Linearnost
$H(a_1 x_1 + a_2 x_2) = a_1H(x_1) + a_2H(x_2)$

## Laplaceova transformacija

| $f(t)$ | $\mathcal{L}({f(t)})=F(s)$ |
|:---:|:---:|
| $1$| $\dfrac{1}{s}$|
| $e^{at}f(t)$	| $F(s-a)$	|
| $\mathcal{U}(t-a)$ | $\dfrac{e^{-as}}{s}$ |
| $f(t-a)\mathcal{U}(t-a)$ | $e^{-as}F(s)$ |
| $\delta(t)$	| 1 |
| $\delta(t-t_0)$ | $e^{-st_0}$ |
| $t^nf(t)$ 	| $(-1)^n\dfrac{d^nF(s)}{ds^n}$  |
| $f'(t)$ 	| $sF(s) - f(0)$ |
| $f^{n}(t)$ 	| $s^nF(s) - s^{(n-1)} f(0) - ... - f^{(n-1)}(0)$ |
| $\displaystyle{\int_0^t f(x)g(t-x)dx}$ | $F(s)G(s)$ |
| $t^n$ ($n=0,1,2,\dots$)     | $\dfrac{n!}{s^{n+1}}$    |
| $t^x$ ($x\geq-1\in\mathbb{R}$)     | $\dfrac{\Gamma(x+1)}{s^{x+1}}$ |
| $\sin kt$ 	| $\dfrac{k}{s^2+k^2}$ |
| $\cos kt$ 	| $\dfrac{s}{s^2+k^2}$ |
| $e^{at}$ 	| $\dfrac{1}{s-a}$ 	|
| $\sinh kt$	| $\dfrac{k}{s^2-k^2}$ |
| $\cosh kt$	| $\dfrac{s}{s^2-k^2}$ |
| $\dfrac{e^{at}-e^{bt}}{a-b}$	| $\dfrac{1}{(s-a)(s-b)}$ |
