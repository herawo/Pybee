# Les conditions
On peut interoger la valeur d'une variable

```python
ma_variable = 1
if ma_variables == 1:
    print('ca passe ici')
elif ma_variables >= 2:
    print('ca ne passe pas ici')
else:
    print('ici non plus')
```
cela introduit la notion de "bloc" de code marqué par les tabulations.

par exemple:
```python
ma_variable = 'toto'
if ma_variable == 'toto':
print('ca passe ici')
```

ne marchera pas, car après un if, le code attend un bloc de code propre au if qui s'executera si la vérification est valide. un bloc se défini par un nombre de tabulation. Pour continuer sortir du bloc, et continuer l'execution normale, on retire des tabulations 

```python
ma_variable = 'toto'
if ma_variable == 'toto':
    print('ca passe ici')
print('ca passe ici aussi')
```

Depuis le début on parle de vérification. En fait c'est un prédicat booléen. Une prédicat c'est un assertion qui va renvoyer vrai ou faux.
exemple:  
```python
beau = True
gentil = False
if beau and not gentil:
    print('vous êtes beau mais pas gentil')
```
cela introduit les opérateurs booléen -> and, or et not
not -> inverse
or -> ou inclusif
and -> et
(voir les tables de calcul booléens)
