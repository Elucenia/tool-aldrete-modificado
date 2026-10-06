<!-- ELUCENIA technical documentation · aldrete-modificado · de · no clinical/professional/rights approval -->

# Modifizierter Aldrete-Score

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/aldrete-modificado)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Motorische Aktivität

`atividade`

- `0` — Keine Bewegung
- `1` — Bewegt 2 Gliedmaßen
- `2` — Bewegt alle 4 Gliedmaßen

### Atmung

`resp`

- `0` — Apnoe
- `1` — Dyspnoe oder eingeschränkte Atmung
- `2` — Atmet tief und hustet

### Kreislauf (Blutdruck im Vergleich zum Wert vor Anästhesie)

`circ`

- `0` — Abweichung ≥ 50 %
- `1` — Abweichung von 20 bis 49 %
- `2` — Variation ≤ 20 %

### Bewusstsein

`consc`

- `0` — Reagiert nicht
- `1` — Erwacht auf Ansprache
- `2` — Vollständig wach

### O₂-Sättigung

`spo2`

- `0` — \< 90 % auch mit O₂
- `1` — Benötigt O₂ zum Halten von \> 90 %
- `2` — \> 92 % unter Raumluft

## Fassung der Methode

Modifizierter Aldrete 1995: 5 Items 0–2, SpO₂ statt Hautfarbe, gesamt 0–10

## Dokumentierte Formel

Fünf Items mit 0–2 Punkten (gesamt 0–10): Aktivität, Atmung, Kreislauf, Bewusstsein und O₂-Sättigung. Die Version 1995 ersetzte Hautfarbe durch Pulsoxymetrie.

## Grenzen und Population

Diese Oberfläche summiert die fünf Komponenten des modifizierten Aldrete zur Erholung nach Anästhesie zu einer Gesamtsumme von 0 bis 10; sie implementiert nicht das erweiterte ambulante Instrument mit zehn Faktoren. Die Gesamtsumme allein erlaubt keine Entlassung und muss durch klinische Beurteilung und erneute Beurteilung ergänzt werden. Die Originaltabellen von 1995 und die Anpassung des Autors von 2007 unterscheiden sich in der Formulierung der Kreislaufgrenzen; genau 20 % bleibt mehrdeutig. Die Tabellen von 1995 unterscheiden sich auch in der niedrigsten Bewertung der Oxygenierung. Diese Unterschiede erfordern eine klinische Klärung und erlauben es nicht, allein aufgrund der Summe vollständige Gleichwertigkeit zu behaupten.

## Referenzen

- [Aldrete JA. The post-anesthesia recovery score revisited. J Clin Anesth, 1995.](https://doi.org/10.1016/0952-8180(94)00001-K)

- [Aldrete JA, Kroulik D. A postanesthetic recovery score. Anesth Analg, 1970.](https://doi.org/10.1213/00000539-197011000-00020)

- [JAntonioAldrete2007,RAA65(3),pp194–195](https://www.anestesia.org.ar/search/articulos_completos/1/1/1121/c.pdf)

- [Aldrete1995,originalletter,reproducedmirror](https://anest-rean.ru/wp-content/uploads/2024/11/Aldrete-J.A.-The-post-anesthesia-recovery-score-revisited.1995.pdf)

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

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Entlassungskriterium für den Aufwachraum erreicht (≥ 9)

Bestätigen Sie außerdem kontrollierte Schmerzen, fehlende oder leichte Übelkeit und das Fehlen aktiver Blutung.


### 2

Entlassungskriterium für den Aufwachraum erreicht (≥ 9)

Bestätigen Sie außerdem kontrollierte Schmerzen, fehlende oder leichte Übelkeit und das Fehlen aktiver Blutung.


### 3

Unter 9: im Aufwachraum belassen

Alle 15 Minuten erneut beurteilen und behandeln, was die Entlassung verhindert (Schmerzen, Hypoxämie, Instabilität, Restsedierung).

