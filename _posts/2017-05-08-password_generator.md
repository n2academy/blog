---
layout: post
title: Password Generator
date:   2017-05-08 12:00:00
categories: posts
---

Shkruani nje funksion qe gjeneron passworde. Mundohuni te jeni kreativë ne gjenerimin e passwordeve. Passwordi duhet te jete i rastesishem, pra funksioni duhet te ktheje nje password te ri cdo here qe therritet, dhe i sigurte.

Seksionet:
1. Importimi i moduleve
2. moduli `random`
3. Cfare duhet dorezuar


## Importim i moduleve

Python vjen i pajisur me nje sere modulesh te ndertuar nga zhvilluesit e
gjuhes dhe komuniteti. Nje modul eshte nje grupim funksionesh qe mund te
perdoren ne kontekste te ndryshme. Modulet mund te importohen me komanden
`import <emri_i_modulit>`. Per shembull, modulin `random` mund te importohet
nepermjet komandes `import random`. Kjo i jep akses programit tuaj ne gjithe
funksionet qe perkfuzohen brenda modulit `random`


## Moduli `random`

Moduli `random` permban nje sere funksionesh qe sherbejne per te gjeneruar
rezultate te rastesishme. Per nje hyrje, shihni shembujt me poshte.
Dokumentacionin e plote te modulit `random` mund ta gjeni ketu:
https://docs.python.org/2/library/random.html

```python
import random # nga ky moment mund te perdorni funksionet e modulit random

a = random.randint(1, 10) # a eshte nje numer i rastesishem nga 1 deri ne 10
print a # printoni a per ta verifikuar

ls = ['1', '2', '3', 'a', 'b']
x = random.choice(ls) # x eshte nje element i rastesishem nga lista ls
print x # printoni x per ta verifikuar
```

## Cfare duhet dorezuar.

Nje file me emrin `password_generator.py` dhe permban nje funksion me emrin `generate`, qe
merr 1 argument `n`: gjatesine e password-it dhe kthen 1 `string` te
rastesishem, sa me te veshtire per tu marre me mend dhe me gjatesi `n`.

Shembull:

  ```python
    def generate(n):
        ...
        ...

    # generate(4) => 'a83s'
    # generate(4) => 'cvD0'
    # generate(6) => '@(3$-)'
    # generate(6) => 'as932_'
  ```
