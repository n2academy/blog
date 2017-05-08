---
layout: post
title: Pjestuesit
date:   2017-05-08 12:00:00
categories: posts
---

Shkruani nje funksion qe merr nje numer te plote (`int`) dhe printon
gjithe pjestuesit e atij numri. (`a` eshte pjestues i `b` nese pjestimi `b/a`
e ka mbetjen `0`)

Mbetja e nje pjestimi ne python mund te perftohet nepermjet operatorit `%`.

Pra `6 % 2` eshte `0`, sepse mbetja e pjestimit `6/2` eshte `0`. `7 % 2` eshte `1`.

## Cfare duhet dorezuar

Nje file me emrin `divisors.py` qe permban nje funksion me emrin `divisors`, i
cili merr nje numer `n` dhe printon gjithe pjestuesit e `n`.

```python
def divisors(n):
    ...
    ...
    ...

# divisors(4)
# 1
# 2
# 4
# divisors(6)
# 1
# 2
# 3
# 6
# divisors(7)
# 1
# 7
```
