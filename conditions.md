# Les conditions

## Interroger une valeur
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
Bien sûr ici et dans les exemple suivant, les verifications seront faite sur des variables qui sont déclarées juste au dessus. L'utilité d'une vérification est de pouvoir gérer des variables dont on ne connait pas le contenu (car il est ... variable)
Cela introduit la notion de "bloc" de code marqué par les tabulations.

## Bloc de code
par exemple:
```python
ma_variable = 'toto'
if ma_variable == 'toto':
print('ca ne précompile meme pas')
```

ne marchera pas, car après un if, le code attend un bloc de code propre au if qui s'executera si la vérification est valide. Un bloc se défini par un nombre de tabulation. Pour sortir du bloc, et continuer l'execution normale, on retire des tabulations 

```python
ma_variable = 'toto'
if ma_variable == 'toto':
    print('ca passe ici')
print('ca passe ici aussi')
```


## Prédicat booléen
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

| A | not A | B | A or B | A and B |
|---|-------|---|--------|---------|
| F | V     | F | F      | F       |
| V | F     | F | V      | F       |
| F |       | V | V      | F       |
| V |       | V | V      | V       |

Un prédicat peut être composé de plusieurs sous prédicat, exemple : `A and B or C and not D`  
en code cela peut se traduire en :
```python
nom = 'Billy'
prenom = 'Bob'
age = 25
taille = 1.5f
if nom.contains('B') and prenom.startswith('B') or age > 20 and not taille < 1:
    print('ça passe ici')
```
on retrouve ici `A and B or C and not D` avec 
- A : `nom.contains('B')` (ici, contains() renvoie True si 'B' est trouvé dans `nom`)
- B : `prenom.startswith('B')` (ici, startswith() renvoie True si 'B' est la premiere lettre dans `prenom`)
- C : `age > 20`
- D : `taille < 1`

On avait dit dans la [partie précédente](variables.md#et-beaucoup-dautres-choses-possibles) qu'une variable peut contenir plein de choses. Elles peuvent notament contenir un prédicat. Exemple :
```python
couleur = 'orange'
animal = 'chat'
mon_predicat = animal == 'chat' and couleur == 'orange'
if mon_predicat:
    print('Je vais l'appeler Garfield')
```

