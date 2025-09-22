
# Accès aux données CMEMS

## Introduction

{abbr}`CMEMS (Copernicus Marine Environment Monitoring Service)` est le service marin du programme Copernicus. Il fournit un **accès libre et gratuit** à des données sur l’océan mondial. Une {abbr}`API (Application Programming Interface)` Python permet l'accès aux données[^1].

[^1]: Pour plus d’informations sur l’installation et l’utilisation de l’API Python, consultez la [documentation CMEMS Toolbox](https://toolbox-docs.marine.copernicus.eu/en/stable/).

## Liste des variables

1. Variables physiques
    * Température
    * Salinité
    * Niveau de la mer
2. Variables biogéochimiques
    * Chlorophylle
    * Oxygène dissous
    * Nutriments

## Exemple de code Python

```python
import copernicusmarine

copernicusmarine.subset(
    dataset_id = "cmems_mod_glo_phy-thetao_anfc_0.083deg_P1D-m",
    variables = ["thetao"],
)
```

```{warning}
Il est nécessaire de s'identifier au préalable avec la commande `copernicusmarine.login()`
```

## FAQ

````{dropdown} Faut-il installer quelque chose pour utiliser l’API Python ?
Oui, il suffit d’installer le package `copernicusmarine` via pip :  
```bash
pip install copernicusmarine
```
````

````{dropdown} Comment s’authentifier avec l’API Python CMEMS ?
1. **Créer un compte** sur le site CMEMS (si ce n’est pas déjà fait).

2. **Se connecter depuis Python** :  
```python
import copernicusmarine

copernicusmarine.login()
```
Une fenêtre ou une invite vous demandera vos identifiants CMEMS. 
````
