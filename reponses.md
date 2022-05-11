# Réponses

## For

## While

```python
fn0 = 0
fn1 = 1
fn2 = fn1 + fn0

compteur = 0

while fn2 < 80000000000:
    fn2 = fn2 + fn1
    fn1 = fn2
    compteur = compteur + 1
print(compteur)
```
