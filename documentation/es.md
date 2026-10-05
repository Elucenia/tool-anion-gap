<!-- ELUCENIA technical documentation · anion-gap · es · no clinical/professional/rights approval -->

# Brecha aniónica (corregida y delta-delta)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/anion-gap)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Sodio

`na`

mEq/L · intervalo: 100–180

### Cloruro

`cl`

mEq/L · intervalo: 60–140

### Bicarbonato

`hco3`

mEq/L · intervalo: 2–50

### Albúmina

`alb`

g/dL · opcional · intervalo: 0,5–6

## Edición del método

AG sin K+; corrección Figge 1998 2,5×(4−albúmina); referencia delta AG 12/delta HCO₃ 24

## Fórmula documentada

Brecha aniónica = Na⁺ − (Cl⁻ + HCO₃⁻).

Corregida por albúmina = AG + 2,5 × (4,0 − albúmina en g/dL).

Razón delta = (AG − 12) ÷ (24 − HCO₃⁻).

## Límites y población

El valor de referencia de la brecha aniónica depende del método de laboratorio y varía entre personas. Los valores alterados no identifican una causa única y pueden reflejar un error de laboratorio. La razón ΔAG/ΔHCO3 no debe utilizarse de forma aislada para identificar trastornos acidobásicos mixtos; se necesitan datos clínicos y de laboratorio adicionales. La corrección por albúmina y los valores de referencia utilizados en el cálculo deben comprobarse en las fuentes de la variante.

## Referencias

- [Kraut JA, Madias NE. Serum anion gap: its uses and limitations in clinical medicine. Clin J Am Soc Nephrol, 2007.](https://doi.org/10.2215/CJN.03020906)

- [Figge J, Jabor A, Kazda A, Fencl V. Anion gap and hypoalbuminemia. Crit Care Med, 1998.](https://doi.org/10.1097/00003246-199811000-00019)

- [Rastegar A. Use of the ΔAG/ΔHCO3− ratio in the diagnosis of mixed acid-base disorders. J Am Soc Nephrol, 2007.](https://doi.org/10.1681/ASN.2006121408)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
