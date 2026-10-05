<!-- ELUCENIA technical documentation · anion-gap · de · no clinical/professional/rights approval -->

# Anionenlücke (korrigiert und Delta-Delta)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/anion-gap)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Natrium

`na`

mEq/L · Bereich: 100–180

### Chlorid

`cl`

mEq/L · Bereich: 60–140

### Bikarbonat

`hco3`

mEq/L · Bereich: 2–50

### Albumin

`alb`

g/dL · optional · Bereich: 0,5–6

## Fassung der Methode

AG ohne K+; Figge-Korrektur 1998 2,5×(4−Albumin); Delta-AG-Referenz 12/Delta-HCO₃-Referenz 24

## Dokumentierte Formel

Anionenlücke = Na⁺ − (Cl⁻ + HCO₃⁻).

Albuminkorrigiert = AG + 2,5 × (4,0 − Albumin in g/dL).

Delta-Ratio = (AG − 12) ÷ (24 − HCO₃⁻).

## Grenzen und Population

Der Referenzwert der Anionenlücke hängt von der Labormethode ab und unterscheidet sich zwischen Personen. Abweichende Werte zeigen keine eindeutige Ursache an und können auf Laborfehler zurückgehen. Das Verhältnis ΔAG/ΔHCO3 darf nicht allein zur Erkennung gemischter Säure-Basen-Störungen verwendet werden; zusätzliche klinische und Labordaten sind erforderlich. Albuminkorrektur und die verwendeten Referenzwerte müssen in den Quellen der jeweiligen Variante geprüft werden.

## Referenzen

- [Kraut JA, Madias NE. Serum anion gap: its uses and limitations in clinical medicine. Clin J Am Soc Nephrol, 2007.](https://doi.org/10.2215/CJN.03020906)

- [Figge J, Jabor A, Kazda A, Fencl V. Anion gap and hypoalbuminemia. Crit Care Med, 1998.](https://doi.org/10.1097/00003246-199811000-00019)

- [Rastegar A. Use of the ΔAG/ΔHCO3− ratio in the diagnosis of mixed acid-base disorders. J Am Soc Nephrol, 2007.](https://doi.org/10.1681/ASN.2006121408)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026
