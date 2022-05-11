# Les boucles

On peut utiliser des structures pour executer plusieurs fois le même code. Chaque passage s'appelle une itération, lorsqu'on a fini une itération on passe a la suivante, jusqu'a ce qu'il n'y ait plus d'itération a faire. 

## For
Utilisé quand on sait combien d'itération on va faire. Par exemple si on veut faire une vérification sur tous les éléments d'une liste. Exemple:
```python
ma_liste = [1, 3, 10 2, 131, -20]
for elem in ma_liste:
    if elem % 2 == 0:
        print("pair")
    else:
        print("impair")
```
Dans l'exemple précédent : 
- % c'est un modulo, un opérateur tout comme le + (addition), le - (soustraction), le * (multiplication) et le / (division). Le modulo permet de retourner le reste de la division euclidienne.
- elem est une nouvelle variable qui va changer de valeur a chaque itération. 
- comme ma_liste est une liste (une collection indéxée, donc ordonnée), on sait que les valeurs de elem respecteront l'ordre dans lequel on les a déclaré.

On peut forcer le passage a l'itération suivante avec `continue` ou completement quitter le for avec `break`.
```python
ma_liste = [1, 3, "passe", 10 2, 131, -20, "fin", 14]
for elem in ma_liste:
    if elem == "passe":
        continue
    elif elem == "fin":
        break
    elif elem % 2 == 0:
        print("pair")
    else:
        print("impair")
```

## While
