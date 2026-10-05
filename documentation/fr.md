<!-- ELUCENIA technical documentation · indice-de-van-nuys · fr · no clinical/professional/rights approval -->

# Indice pronostique de Van Nuys (USC/VNPI)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/indice-de-van-nuys)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Taille du carcinome canalaire in situ

`tam`

- `1` — ≤ 15 mm
- `2` — 16 à 40 mm
- `3` — ≥ 41 mm

### Plus petite marge saine

`margem`

- `1` — ≥ 10 mm
- `2` — 1 à 9 mm
- `3` — \< 1 mm

### Classification anatomopathologique

`pato`

- `1` — Non haut grade, sans nécrose
- `2` — Non haut grade, avec nécrose
- `3` — Haut grade (avec ou sans nécrose)

### Âge

`idade`

- `1` — \> 60 ans
- `2` — 40 à 60 ans
- `3` — \< 40 ans

## Édition de la méthode

USC/VNPI/Silverstein 2003 : 4 facteurs avec âge, total 4–12 ; pas VNPI à 3 facteurs

## Formule documentée

Somme de 4 facteurs, chacun 1–3 : taille, marge minimale, classification pathologique (grade nucléaire, nécrose comédo), âge. Total 4–12.

## Limites et population

L’USC/VNPI 2003 a été étudié dans le CCIS pur traité par chirurgie conservatrice et ajoute l’âge aux trois facteurs précédents. Ce n’est pas l’indice original à trois facteurs et il ne doit pas être automatiquement appliqué au carcinome invasif. Les suggestions de traitement reflètent la base décrite et nécessitent une évaluation clinique et des preuves contemporaines.

## Références

- [Silverstein MJ. The University of Southern California/Van Nuys prognostic index for ductal carcinoma in situ of the breast. Am J Surg, 2003.](https://doi.org/10.1016/S0002-9610(03)00265-4)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
