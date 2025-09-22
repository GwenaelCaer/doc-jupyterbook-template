
Accès aux données CMEMS

Introduction

CMEMS (Copernicus Marine Environment Monitoring Service est le service marin du programme Copernicus. Il fournit un accès libre et gratuit à des données sur l’océan mondial. Une API (Application Programming Interface) Python permet l'accès aux données (https://toolbox-docs.marine.copernicus.eu/en/stable/).


Liste des variables

Variables physiques (Température, Salinité, Niveau de la mer) et variables biogéochimiques (Chlorophylle, Oxygène dissous, Nutriments)

Exemple de code Python

import copernicusmarine

copernicusmarine.subset(
    dataset_id = "cmems_mod_glo_phy-thetao_anfc_0.083deg_P1D-m",
    variables = ["thetao"],
)

Attention: Il est nécessaire de s'identifier au préalable avec la commande copernicusmarine.login()

FAQ

Q: Faut-il installer quelque chose pour utiliser l’API Python ?
R: Oui, il suffit d’installer le package copernicusmarine via pip : pip install copernicusmarine

Q: Comment s’authentifier avec l’API Python CMEMS ?
R: Créer un compte sur le site CMEMS (si ce n’est pas déjà fait). Puis se connecter depuis Python: 

import copernicusmarine

copernicusmarine.login()

Une fenêtre ou une invite vous demandera vos identifiants CMEMS. 

