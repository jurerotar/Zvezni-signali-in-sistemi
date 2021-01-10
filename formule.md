﻿
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

### Eksponenta vrsta

$A_n=\frac{1}{T} \int_{0}^T f(x) \cdot e^{-jn \pi x} dx$

$x(t)=a_0 + \sum_{n \neq 0} A_n$

#### Zveze

$e^{-j \pi n}=(-1)^n$



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