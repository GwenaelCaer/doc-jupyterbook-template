CMEMS (Copernicus Marine Environment Monitoring Service) est le service marin du programme Copernicus. Il fournit un accès libre et gratuit à des données, produits et informations sur l’océan mondial et les mers régionales. Une API (Application Programming Interface) Python permet l'accès aux données (https://toolbox-docs.marine.copernicus.eu/en/stable/).



```{myst}
{abbr}`CMEMS (Copernicus Marine Environment Monitoring Service)` est le service marin du programme Copernicus. Il fournit un **accès libre et gratuit** à des données, produits et informations sur l’océan mondial et les mers régionales. Une {abbr}`API (Application Programming Interface)` Python permet l'accès aux données[^1].

[^1]: Pour plus d’informations sur l’installation et l’utilisation de l’API Python, consultez la [documentation CMEMS Toolbox](https://toolbox-docs.marine.copernicus.eu/en/stable/).
```

```markdown
CMEMS (Copernicus Marine Environment Monitoring Service est le service marin du programme Copernicus. Il fournit un accès libre et gratuit à des données sur l’océan mondial.
```


# Accès aux données CMEMS

## Introduction

```markdown
CMEMS (Copernicus Marine Environment Monitoring Service est le service marin du programme Copernicus. Il fournit un accès libre et gratuit à des données sur l’océan mondial.
```

`CMEMS` (_Copernicus Marine Environment Monitoring Service_) est le service marin du programme Copernicus. Il fournit un **accès libre et gratuit** à des données sur l’océan mondial.

```markdown
Une API (Application Programming Interface) Python permet l'accès aux données (https://toolbox-docs.marine.copernicus.eu/en/stable/).
```

```markdown
Variables physiques (Température, Salinité, Niveau de la mer) et variables biogéochimiques (Chlorophylle, Oxygène dissous, Nutriments)
```

1. Variables physiques
    * Température
    * Salinité
    * Niveau de la mer
2. Variables biogéochimiques
    * Chlorophylle
    * Oxygène dissous
    * Nutriments

```markdown
import copernicusmarine
copernicusmarine.subset(
    dataset_id = "cmems_mod_glo_phy-thetao_anfc_0.083deg_P1D-m",
    variables = ["thetao"],
)
```

```python
import copernicusmarine

copernicusmarine.subset(
    dataset_id = "cmems_mod_glo_phy-thetao_anfc_0.083deg_P1D-m",
    variables = ["thetao"],
)
```

```markdown
Il est nécessaire de s'identifier au préalable avec la commande `copernicusmarine.login()`
```

```{warning}
Il est nécessaire de s'identifier au préalable avec la commande `copernicusmarine.login()`
```

```markdown
Q: Faut-il installer quelque chose pour utiliser l’API Python ?
R: Oui, il suffit d’installer le package copernicusmarine via pip : pip install copernicusmarine
```


````{dropdown} Faut-il installer quelque chose pour utiliser l’API Python ?
Oui, il suffit d’installer le package `copernicusmarine` via pip :  
```bash
pip install copernicusmarine
```
````


# TEST





Une {abbr}`API (Application Programming Interface)` Python permet l'accès aux données[^1].

[^1]: Pour plus d’informations sur l’installation et l’utilisation de l’API Python, consultez la [documentation CMEMS Toolbox](https://toolbox-docs.marine.copernicus.eu/en/stable/).