<!-- ELUCENIA technical documentation · anion-gap · fr · no clinical/professional/rights approval -->

# Trou anionique (corrigé et delta-delta)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/anion-gap)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Sodium

`na`

mEq/L · intervalle: 100–180

### Chlorure

`cl`

mEq/L · intervalle: 60–140

### Bicarbonate

`hco3`

mEq/L · intervalle: 2–50

### Albumine

`alb`

g/dL · facultatif · intervalle: 0,5–6

## Édition de la méthode

AG sans K+ ; correction Figge 1998 2,5×(4−albumine) ; références delta AG 12/delta HCO₃ 24

## Formule documentée

Trou anionique = Na⁺ − (Cl⁻ + HCO₃⁻).

Corrigé pour l’albumine = AG + 2,5 × (4,0 − albumine en g/dL).

Rapport delta = (AG − 12) ÷ (24 − HCO₃⁻).

## Limites et population

La valeur de référence du trou anionique dépend de la méthode de laboratoire et varie d’une personne à l’autre. Des valeurs anormales n’identifient pas une cause unique et peuvent traduire une erreur de laboratoire. Le rapport ΔAG/ΔHCO3 ne doit pas être utilisé seul pour identifier des troubles acido-basiques mixtes ; des données cliniques et biologiques supplémentaires sont nécessaires. La correction pour l’albumine et les valeurs de référence utilisées dans le calcul doivent être vérifiées dans les sources de la variante.

## Références

- [Kraut JA, Madias NE. Serum anion gap: its uses and limitations in clinical medicine. Clin J Am Soc Nephrol, 2007.](https://doi.org/10.2215/CJN.03020906)

- [Figge J, Jabor A, Kazda A, Fencl V. Anion gap and hypoalbuminemia. Crit Care Med, 1998.](https://doi.org/10.1097/00003246-199811000-00019)

- [Rastegar A. Use of the ΔAG/ΔHCO3− ratio in the diagnosis of mixed acid-base disorders. J Am Soc Nephrol, 2007.](https://doi.org/10.1681/ASN.2006121408)

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

Trou anionique normal


### 2

Trou anionique normal : s’il existe une acidose métabolique, elle est hyperchlorémique


### 3

Trou anionique augmenté : acidose métabolique due à des anions non mesurés (lactate, cétones, urémie, toxiques)

| Détails du résultat | |
| --- | --- |
| Trou anionique corrigé pour l’albumine | 30,0 mEq/L |
| Rapport delta (ΔAG/ΔHCO₃⁻) | 1,29 : acidose à trou anionique élevé isolée |


### 4

Trou anionique augmenté : acidose métabolique due à des anions non mesurés (lactate, cétones, urémie, toxiques)

| Détails du résultat | |
| --- | --- |
| Trou anionique corrigé pour l’albumine | 17,0 mEq/L |
| Rapport delta (ΔAG/ΔHCO₃⁻) | 0,83 : acidose à trou anionique élevé associée à une acidose à trou anionique normal |


### 5

Trou anionique augmenté : acidose métabolique due à des anions non mesurés (lactate, cétones, urémie, toxiques)

| Détails du résultat | |
| --- | --- |
| Rapport delta (ΔAG/ΔHCO₃⁻) | 4,50 : acidose à trou anionique élevé associée à une alcalose métabolique (ou à une acidose respiratoire chronique compensée) |

