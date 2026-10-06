<!-- ELUCENIA technical documentation · anion-gap · it · no clinical/professional/rights approval -->

# Gap anionico (corretto e delta-delta)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/anion-gap)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Sodio

`na`

mEq/L · intervallo: 100–180

### Cloruro

`cl`

mEq/L · intervallo: 60–140

### Bicarbonato

`hco3`

mEq/L · intervallo: 2–50

### Albumina

`alb`

g/dL · facoltativo · intervallo: 0,5–6

## Edizione del metodo

AG senza K+; correzione Figge 1998 2,5×(4−albumina); riferimento delta AG 12/delta HCO₃ 24

## Formula documentata

Gap anionico = Na⁺ − (Cl⁻ + HCO₃⁻).

Corretto per albumina = AG + 2,5 × (4,0 − albumina in g/dL).

Rapporto delta = (AG − 12) ÷ (24 − HCO₃⁻).

## Limiti e popolazione

Il valore di riferimento del gap anionico dipende dal metodo di laboratorio e varia tra persone. Valori alterati non identificano un’unica causa e possono riflettere un errore di laboratorio. Il rapporto ΔAG/ΔHCO3 non deve essere usato da solo per identificare disturbi misti dell’equilibrio acido-base; occorrono ulteriori dati clinici e di laboratorio. La correzione per l’albumina e i valori di riferimento utilizzati nel calcolo richiedono una verifica nelle fonti della variante.

## Riferimenti

- [Kraut JA, Madias NE. Serum anion gap: its uses and limitations in clinical medicine. Clin J Am Soc Nephrol, 2007.](https://doi.org/10.2215/CJN.03020906)

- [Figge J, Jabor A, Kazda A, Fencl V. Anion gap and hypoalbuminemia. Crit Care Med, 1998.](https://doi.org/10.1097/00003246-199811000-00019)

- [Rastegar A. Use of the ΔAG/ΔHCO3− ratio in the diagnosis of mixed acid-base disorders. J Am Soc Nephrol, 2007.](https://doi.org/10.1681/ASN.2006121408)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Anion gap normale


### 2

Anion gap normale: se è presente acidosi metabolica, è ipercloremica


### 3

Anion gap aumentato: acidosi metabolica da anioni non misurati (lattato, chetoni, uremia, tossici)

| Dettagli del risultato | |
| --- | --- |
| Anion gap corretto per l’albumina | 30,0 mEq/L |
| Rapporto delta (ΔAG/ΔHCO₃⁻) | 1,29: acidosi con AG alto isolata |


### 4

Anion gap aumentato: acidosi metabolica da anioni non misurati (lattato, chetoni, uremia, tossici)

| Dettagli del risultato | |
| --- | --- |
| Anion gap corretto per l’albumina | 17,0 mEq/L |
| Rapporto delta (ΔAG/ΔHCO₃⁻) | 0,83: acidosi con AG alto associata ad acidosi con AG normale |


### 5

Anion gap aumentato: acidosi metabolica da anioni non misurati (lattato, chetoni, uremia, tossici)

| Dettagli del risultato | |
| --- | --- |
| Rapporto delta (ΔAG/ΔHCO₃⁻) | 4,50: acidosi con AG alto associata ad alcalosi metabolica (o acidosi respiratoria cronica compensata) |

