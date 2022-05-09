# Pybee
projet to learn python

# Les variables

## Déclarer une variable

```python
ma_variable = 1
```

Il existe différent types de variables

### Les entier (int)

exemple: 0; 1; 18; 105902; -87

### Les flotants (float)
tire son nom du principe de la virgule flotante, utilisé pour les nombres décimaux

exemple: 0,48; -50,85; 8; -1000,00
```python
ma_variable = 0.48
```

### Les chaînes de caracteres (string)

matérialisés par des mots entre '' ou ""
exemple: 'c'; "mot"; "je suis beau", '', "38"

### Les booléens (bool)

2 états : True / False

### Les collections

#### Les listes (list)

un ensemble de variables  
exemple:  
```python
un_caractere = 'c'
ma_list = [1, 2, "3", un_caractere, ['lol', True]]
```

on peut accéder aux valeurs grâce a l'index (la position dans la liste). le premier est à l'index 0, le second à l'index 1, etc.  
exemple:  
```python
un_caractere = 'c'
ma_liste = [1, 2, "3", un_caractere]
print(ma_liste[0])
```
(print permet d'afficher une variable)

#### Les tuples (tuple)

Comme une liste mais marquée par des () au lieu des []. La différence est qu'un tuple est immutable. Après instanciation, on ne peut pas modifier le contenu
```python
mon_tuple = (1, 2, 3)
mon_tuple[0] = 10
```
la derniere ligne produira une erreur

#### Les ensembles (set)
Une liste que ne peut pas contenir de doublon
```python
mon_set = set(1, 2, 3)
```

#### Les dictionnaires
Une liste où les index peuvent être des valeurs (là on rentre dans des trucs casse tête) marqué par des {}
```python
mon_dict = {'toto': 1, 2: 'valeur 2', 3: True, 'une liste': ['lol', 1]}
```
On accède pareillement aux valeurs avec l'index.
```python
mon_dict['toto'] 
```  
renvera 1

### Et beaucoup d'autres choses possibles

## Passer d'un type a un autre (le cast)

passage d'entier a chaîne de caractere
exemple :
```python
ma_variable = 1
ma_variable_str = str(ma_variable)
```
ma_variable vaudra 1 alors que ma_variable_str vaudra "1"

à tester le passage de chaque type a un autre, des petites complexités existent comme le fait de devoir passer avant par le float pour passer de la string vers l'int `int(float("14"))`

## Les conditions
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


