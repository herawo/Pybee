# Pybee
projet to learn python

# Les basiques

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
mon_dict = {
    'toto': 1, 2: 'valeur 2', 3: True, 'une liste': ['lol', 1]
}
```
On accède pareillement aux valeurs avec l'index.
```python
mon_dict['toto'] 
```  
renvera 1


