---
layout: post
title: Llogaritja e π
date:   2017-05-08 12:00:00
categories: posts
---

Ne kete ushtrim do eksplorojme llogaritjen me perafersi te vleres se pi.

Ndertojme nje rreth me rreze `r` brenda nje katrori me gjatesi brinje `2r`.

![rreth katror](https://i.imgur.com/GzcWhNR.png "rreth katror")

Ne figure verejme disa detaje:
  1. Siperfaqja e rrethit (blu) eshte `πr²`
  2. Siperfaqja e katrorit gri eshte `2r * 2r = 4r²`
  3. Raporti i siperfaqes se rrethit me siperfaqen e katrorit eshte `raporti = πr²/4r² = π/4`
  4. Keshtu, vlera e `π` eshte `raporti * 4`

Pra, nese arrijme te llogarisim raportin e siperfaqes se rrethit me siperfaqen e katrorit (`raporti`) mund te llogarisim dhe vleren e `π`.

Nje metode statistikore (Monte Carlo simulation) mund te perdoret per te llogaritur kete raport.
Nese gjenerojme nje pike te rastesishme brenda katrorit, probabiliteti qe kjo pike te gjendet brenda rrethit (ne zonen blu) eshte:
```
p = (siperfaqja e rrethit) / (siperfaqja e katrorit) = raporti = π/4
```
Ky probabilitet mund te perafersohet duke gjeneruar nje numer te madh pikash te rastesishme, per shembull:
  1. Gjenero `10000` pika te rastesishme. (nje pike mund te shprehet si 2 variabla `x` dhe `y`
  2. Numero pikat qe bien brenda siperfaqes se rrethit (zona blu)
  3. probabiliteti `p` eshte `p = (pikat qe bien ne zonen blu) / 10000`


## Cfare duhet dorezuar

Nje file qe quhet `pi.py`, dhe permban nje funksion me emrin `pi`
i cili merr si parameter numrin e iterimeve (sa pika te rastesishme duhet te gjenerohen)
dhe kthen nje vlere te perafert te pi (float), duke kryer simulimin e mesiperm me numrin e dhene
te iterimeve.

  ```python
  def pi(iterations):
      ...
      ...

  #pi(10000) => 3.1415...
  ```
