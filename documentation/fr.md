<!-- ELUCENIA technical documentation · aldrete-modificado · fr · no clinical/professional/rights approval -->

# Score d’Aldrete modifié

[conditions, sources et autorisations](https://elucenia.org/fr/outils/aldrete-modificado)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Activité motrice

`atividade`

- `0` — Aucun mouvement
- `1` — Bouge 2 membres
- `2` — Bouge les 4 membres

### Respiration

`resp`

- `0` — Apnée
- `1` — Dyspnée ou respiration limitée
- `2` — Respire profondément et tousse

### Circulation (pression artérielle par rapport à la valeur préanesthésique)

`circ`

- `0` — Variation ≥ 50 %
- `1` — Variation de 20 à 49 %
- `2` — Variation ≤ 20 %

### Conscience

`consc`

- `0` — Ne répond pas
- `1` — S’éveille à l’appel
- `2` — Complètement éveillé

### Saturation en O₂

`spo2`

- `0` — \< 90 % même sous O₂
- `1` — Nécessite de l’O₂ pour maintenir \> 90 %
- `2` — \> 92 % à l’air ambiant

## Édition de la méthode

Aldrete modifié 1995 : 5 items 0–2, SpO₂ remplace la couleur, total 0–10

## Formule documentée

Cinq items cotés 0–2 (total 0–10) : activité, respiration, circulation, conscience et saturation O₂. La version 1995 a remplacé la couleur de peau par l’oxymétrie de pouls.

## Limites et population

Cette interface additionne les cinq composantes de l’Aldrete modifié pour la récupération postanesthésique, avec un total de 0 à 10 ; elle n’implémente pas l’instrument ambulatoire élargi à dix facteurs. Le total isolé n’autorise pas la sortie et doit être accompagné d’une évaluation et d’une réévaluation cliniques. Les tableaux originaux de 1995 et l’adaptation de l’auteur de 2007 diffèrent dans la formulation des limites circulatoires ; exactement 20 % reste ambigu. Les tableaux de 1995 divergent aussi sur la cotation d’oxygénation la plus basse. Ces différences exigent un arbitrage clinique et ne permettent pas d’affirmer une équivalence intégrale sur la seule base de la somme.

## Références

- [Aldrete JA. The post-anesthesia recovery score revisited. J Clin Anesth, 1995.](https://doi.org/10.1016/0952-8180(94)00001-K)

- [Aldrete JA, Kroulik D. A postanesthetic recovery score. Anesth Analg, 1970.](https://doi.org/10.1213/00000539-197011000-00020)

- [JAntonioAldrete2007,RAA65(3),pp194–195](https://www.anestesia.org.ar/search/articulos_completos/1/1/1121/c.pdf)

- [Aldrete1995,originalletter,reproducedmirror](https://anest-rean.ru/wp-content/uploads/2024/11/Aldrete-J.A.-The-post-anesthesia-recovery-score-revisited.1995.pdf)

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

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Critère de sortie de la salle de réveil atteint (≥ 9)

Confirmer également une douleur contrôlée, des nausées absentes ou légères et l’absence de saignement actif.


### 2

Critère de sortie de la salle de réveil atteint (≥ 9)

Confirmer également une douleur contrôlée, des nausées absentes ou légères et l’absence de saignement actif.


### 3

En dessous de 9 : maintenir en salle de réveil

Réévaluer toutes les 15 minutes et traiter ce qui empêche la sortie (douleur, hypoxémie, instabilité, sédation résiduelle).

