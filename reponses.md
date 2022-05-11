# Réponses

## For


```python
import random

randoms = []
for i in range(10):
    randoms.append(random.randint(-10, 10))
print(randoms)
    
for rand1 in randoms:
    for rand2 in randoms:
        if rand1 * rand2 > 0:
            print('positif', rand1 * rand2)
        else:
            print('negatif', rand1 * rand2)
```

Si on veut flex, on peut générer la liste ainsi:
```python
import random
randoms = [random.randint(-10, 10) for i in range(10)]
print(randoms)
```
-> C'est la compréhension de liste, un mécanisme pratique en python permettant d'écrire des itérables (liste, tuples, dictionnaire) sur une ligne

## While

```python
fn0 = 0
fn1 = 1
fn2 = fn1 + fn0

compteur = 0

while fn2 < 5000:
    fn2 = fn2 + fn1
    fn1 = fn2
    compteur = compteur + 1
print(compteur)
```
