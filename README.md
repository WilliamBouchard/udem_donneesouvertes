# HNU6055: Humanités numériques: données ouvertes
Le cours *Humanités numériques : données ouvertes* m'intéresse parce qu'il aborde la question cruciale de l'accès aux données dans la recherche en sciences humaines.

En tant que philologue, ma recherche porte sur **la structuration, la diffusion et l'interopérabilité des corpus numériques** dans le contexte de la littérature grecque ancienne. Ce cours me permettra d’approfondir ma compréhension des principes de transparence, de collaboration et de reproductibilité qui sous-tendent les démarches ouvertes dans le domaine des humanités.

# Projet Toponymes

Dans le cadre du cours HNU6055, je m'intéresse aux variations statistiques entre les origines linguistiques des toponymes désofficialisés par la Commission de toponymie du Québec. 

## Source des données

COMMISSION DE TOPONYMIE. Toponymes désofficialisés, [Jeu de données], dans Données Québec, 2016, mis à jour le 14 mars 2025. [https://www.donneesquebec.ca/recherche/dataset/toponymes-desofficialises], (consulté le 07 mai 2025).

## Organisation du dépôt

## Structure des données

Le fichier des changements de noms aux toponymes répertorie les noms de lieux qui ont déjà été officiels et qui ont été remplacés par un autre nom. En voici la liste des champs.

#### Identifiant
Identifiant de l’ancien nom officiel. 

#### Ancien_nom_officiel
Nom du lieu qui a déjà été officiel, il a été remplacé par le nom dans le champ « Nom_officiel ».
Il est composé de la partie spécifique suivie de la partie générique du toponyme. La partie générique est facultative, si elle est présente elle est séparée de la partie spécifique par une virgule et un espace. Les nombres ordinaux sont exprimés en bas de casse (1er, 1re, 2e, pour premier, première, deuxième, etc.).

#### Identifiant_du_nom_officiel
Identifiant du nom officiel, il est associé au champ « Nom_officiel ». On peut s’en servir pour faire le lien avec les données du fichier des toponymes officiels.
S’il n’y a pas de valeur, c’est que le lieu n’a plus de nom officiel. Conséquemment le champ suivant « Nom_officiel » ne contient pas de valeur.

#### Nom_officiel
Nom du lieu officiel.
Il est composé de la partie spécifique suivie de la partie générique du toponyme. La partie générique est facultative, si elle est présente elle est séparée de la partie spécifique par une virgule et un espace. Les nombres ordinaux sont exprimés en bas de casse (1er, 1re, 2e, pour premier, première, deuxième, etc.).
Cette colonne ne contient pas de valeur si le lieu n’a plus de nom officiel.

#### Type_entite
Nature du lieu nommé.

#### Latitude
Coordonnée géographique du lieu en format décimal pour être utilisé par les systèmes d’information géographique (SIG). Le système de référence géodésique NAD83 est utilisé.

#### Longitude
Coordonnée géographique du lieu en format décimal pour être utilisé par les systèmes d’information géographique (SIG). Le système de référence géodésique NAD83 est utilisé.

#### Feuillet_cartographique
Numéro de la carte topographique à l’échelle 1/50 000, établi selon le système national de référence cartographique (S. N. R. C.) et qui correspond aux coordonnées géographiques où se trouve le toponyme. Par exemple : 21L/11.

### Territoire de municipalité locale
Territoire administratif auquel se rattache le toponyme. Peut être une municipalité locale ou un territoire non organisé.

#### Code_geographique
Identifiant du territoire. Cet identifiant a été attribué par l’Institut de la statistique du Québec.
Il est composé de 5 caractères numériques.

#### Municipalite
Nom du territoire correspondant au code géographique.
Designation

#### Voici la liste des désignations possibles :
    • Établissement amérindien
    • Municipalité
    • Municipalité de canton
    • Municipalité de cantons unis
    • Municipalité de paroisse
    • Municipalité de village
    • Municipalité de village cri
    • Municipalité de village naskapi
    • Municipalité de village nordique
    • Réserve indienne
    • Terres de catégorie 1 pour les Inuits
    • Terres réservées aux Cris
    • Terres réservées aux Naskapis
    • Territoire non organisé
    • Ville

#### Date decision
Date de la réunion des membres de la Commission de toponymie, à laquelle a été déofficialisé le nom.

#### Origine linguistique
Origine linguistique du premier mot spécifique du toponyme. Voici la liste des désignations possibles :
    • Français
    • Anglais
    • Langue amérindienne indéterminée
    • Abénaquis
    • Algonquin
    • Attikamek
    • Cri
    • Malécite
    • Micmac
    • Innu
    • Mohawk
    • Naskapis
    • Wendat
    • Inuktitut
    • Autre
    • Hybride
    • Indifférencié
    • Inconnu

#### Partie_spécifique
Partie spécifique du nom du lieu. La valeur de cette colonne est dérivée de la colonne toponyme. Si le toponyme comporte une virgule, il s’agit de la chaîne de caractères précédant la virgule. Sinon il s’agit du toponyme au complet.

#### Partie_générique
Partie générique du nom du lieu. La valeur de cette colonne est dérivée de la colonne toponyme. Si le toponyme comporte une virgule, il s’agit de la chaîne de caractère suivant la virgule et l’espace. Sinon le champ est vide.


Shield : [![CC BY 4.0][cc-by-shield]][cc-by]

Cette œuvre est mise à disposition selon les termes de la
[licence Creative Commons Attribution 4.0 International][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: https://creativecommons.org/licenses/by/4.0/deed.fr
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
