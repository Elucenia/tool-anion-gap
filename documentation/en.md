<!-- ELUCENIA technical documentation · anion-gap · en · no clinical/professional/rights approval -->

# Anion gap (corrected and delta–delta)

[conditions, sources and permissions](https://elucenia.org/en/tools/anion-gap)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Sodium

`na`

mEq/L · range: 100–180

### Chloride

`cl`

mEq/L · range: 60–140

### Bicarbonate

`hco3`

mEq/L · range: 2–50

### Albumin

`alb`

g/dL · optional · range: 0.5–6

## Method edition

AG without K+; Figge 1998 correction 2.5×(4−albumin); delta AG reference 12/delta HCO₃ reference 24

## Documented formula

Anion gap = Na⁺ − (Cl⁻ + HCO₃⁻).

Albumin-corrected = AG + 2.5 × (4.0 − albumin in g/dL).

Delta ratio = (AG − 12) ÷ (24 − HCO₃⁻).

## Limits and population

The reference value for the anion gap depends on the laboratory method and varies between individuals. Abnormal values do not identify a single cause and may reflect laboratory error. The ΔAG/ΔHCO3 ratio should not be used alone to identify mixed acid–base disorders; additional clinical and laboratory data are needed. Albumin correction and the reference values used in the calculation require checking against the sources for the variant.

## References

- [Kraut JA, Madias NE. Serum anion gap: its uses and limitations in clinical medicine. Clin J Am Soc Nephrol, 2007.](https://doi.org/10.2215/CJN.03020906)

- [Figge J, Jabor A, Kazda A, Fencl V. Anion gap and hypoalbuminemia. Crit Care Med, 1998.](https://doi.org/10.1097/00003246-199811000-00019)

- [Rastegar A. Use of the ΔAG/ΔHCO3− ratio in the diagnosis of mixed acid-base disorders. J Am Soc Nephrol, 2007.](https://doi.org/10.1681/ASN.2006121408)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

Normal anion gap


### 2

Normal anion gap: if there is metabolic acidosis, it is hyperchloremic


### 3

Increased anion gap: metabolic acidosis due to unmeasured anions (lactate, ketones, uremia, toxins)

| Result details | |
| --- | --- |
| Anion gap corrected for albumin | 30.0 mEq/L |
| Delta ratio (ΔAG/ΔHCO₃⁻) | 1.29: isolated high-AG acidosis |


### 4

Increased anion gap: metabolic acidosis due to unmeasured anions (lactate, ketones, uremia, toxins)

| Result details | |
| --- | --- |
| Anion gap corrected for albumin | 17.0 mEq/L |
| Delta ratio (ΔAG/ΔHCO₃⁻) | 0.83: high-AG acidosis associated with normal-AG acidosis |


### 5

Increased anion gap: metabolic acidosis due to unmeasured anions (lactate, ketones, uremia, toxins)

| Result details | |
| --- | --- |
| Delta ratio (ΔAG/ΔHCO₃⁻) | 4.50: high-AG acidosis associated with metabolic alkalosis (or compensated chronic respiratory acidosis) |

