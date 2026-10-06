<!-- ELUCENIA technical documentation · anion-gap · pt-BR · no clinical/professional/rights approval -->

# Ânion gap (corrigido e delta-delta)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/anion-gap)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Sódio

`na`

mEq/L · intervalo: 100–180

### Cloro

`cl`

mEq/L · intervalo: 60–140

### Bicarbonato

`hco3`

mEq/L · intervalo: 2–50

### Albumina

`alb`

g/dL · opcional · intervalo: 0,5–6

## Edição do método

AG sem K+; correção Figge 1998 2,5×(4−albumina); delta AG 12/delta HCO 3 24

## Fórmula documentada

Ânion gap = Na⁺ − (Cl⁻ + HCO₃⁻).

Corrigido pela albumina = AG + 2,5 × (4,0 − albumina em g/dL).

Razão delta = (AG − 12) ÷ (24 − HCO₃⁻).

## Limites e população

O valor de referência do ânion gap depende do método laboratorial e apresenta variabilidade entre pessoas. Valores alterados não identificam uma causa única e podem refletir erro de laboratório. A razão ΔAG/ΔHCO3 não deve ser usada isoladamente para identificar distúrbios ácido-base mistos; são necessários dados clínicos e laboratoriais adicionais. A correção por albumina e os valores de referência usados no cálculo requerem conferência nas fontes da variante.

## Referências

- [Kraut JA, Madias NE. Serum anion gap: its uses and limitations in clinical medicine. Clin J Am Soc Nephrol, 2007.](https://doi.org/10.2215/CJN.03020906)

- [Figge J, Jabor A, Kazda A, Fencl V. Anion gap and hypoalbuminemia. Crit Care Med, 1998.](https://doi.org/10.1097/00003246-199811000-00019)

- [Rastegar A. Use of the ΔAG/ΔHCO3− ratio in the diagnosis of mixed acid-base disorders. J Am Soc Nephrol, 2007.](https://doi.org/10.1681/ASN.2006121408)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Ânion gap normal


### 2

Ânion gap normal: se há acidose metabólica, ela é hiperclorêmica


### 3

Ânion gap aumentado: acidose metabólica por ânions não medidos (lactato, cetonas, uremia, tóxicos)

| Detalhes do resultado | |
| --- | --- |
| Ânion gap corrigido pela albumina | 30,0 mEq/L |
| Razão delta (ΔAG/ΔHCO₃⁻) | 1,29: acidose com AG alto isolada |


### 4

Ânion gap aumentado: acidose metabólica por ânions não medidos (lactato, cetonas, uremia, tóxicos)

| Detalhes do resultado | |
| --- | --- |
| Ânion gap corrigido pela albumina | 17,0 mEq/L |
| Razão delta (ΔAG/ΔHCO₃⁻) | 0,83: acidose com AG alto associada a acidose com AG normal |


### 5

Ânion gap aumentado: acidose metabólica por ânions não medidos (lactato, cetonas, uremia, tóxicos)

| Detalhes do resultado | |
| --- | --- |
| Razão delta (ΔAG/ΔHCO₃⁻) | 4,50: acidose com AG alto associada a alcalose metabólica (ou acidose respiratória crônica compensada) |

