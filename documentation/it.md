<!-- ELUCENIA technical documentation · aldrete-modificado · it · no clinical/professional/rights approval -->

# Indice di Aldrete modificato

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/aldrete-modificado)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Attività motoria

`atividade`

- `0` — Nessun movimento
- `1` — Muove 2 arti
- `2` — Muove tutti e 4 gli arti

### Respirazione

`resp`

- `0` — Apnea
- `1` — Dispnea o respirazione limitata
- `2` — Respira profondamente e tossisce

### Circolazione (pressione arteriosa rispetto al valore preanestetico)

`circ`

- `0` — Variazione ≥ 50%
- `1` — Variazione dal 20 al 49%
- `2` — Variazione ≤ 20%

### Coscienza

`consc`

- `0` — Non risponde
- `1` — Si sveglia alla chiamata
- `2` — Completamente sveglio

### Saturazione di O₂

`spo2`

- `0` — \< 90% anche con O₂
- `1` — Necessita di O₂ per mantenere \> 90%
- `2` — \> 92% in aria ambiente

## Edizione del metodo

Aldrete modificato 1995: 5 item 0–2, SpO₂ al posto del colore, totale 0–10

## Formula documentata

Cinque item da 0–2 punti (totale 0–10): attività, respirazione, circolazione, coscienza e saturazione O₂. La versione 1995 sostituisce il colore cutaneo con pulsossimetria.

## Limiti e popolazione

Questa interfaccia somma i cinque componenti dell’Aldrete modificato per il recupero postanestetico, con un totale da 0 a 10; non implementa lo strumento ambulatoriale ampliato a dieci fattori. Il totale isolato non autorizza la dimissione e deve essere accompagnato da valutazione e rivalutazione clinica. Le tabelle originali del 1995 e l’adattamento dell’autore del 2007 differiscono nella formulazione dei limiti circolatori; esattamente 20% rimane ambiguo. Le tabelle del 1995 differiscono anche nel punteggio più basso di ossigenazione. Queste differenze richiedono un’adjudicazione clinica e non consentono di affermare un’equivalenza integrale solo sulla base della somma.

## Riferimenti

- [Aldrete JA. The post-anesthesia recovery score revisited. J Clin Anesth, 1995.](https://doi.org/10.1016/0952-8180(94)00001-K)

- [Aldrete JA, Kroulik D. A postanesthetic recovery score. Anesth Analg, 1970.](https://doi.org/10.1213/00000539-197011000-00020)

- [JAntonioAldrete2007,RAA65(3),pp194–195](https://www.anestesia.org.ar/search/articulos_completos/1/1/1121/c.pdf)

- [Aldrete1995,originalletter,reproducedmirror](https://anest-rean.ru/wp-content/uploads/2024/11/Aldrete-J.A.-The-post-anesthesia-recovery-score-revisited.1995.pdf)

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

Criterio di dimissione dalla sala di risveglio raggiunto (≥ 9)

Confermare anche dolore controllato, nausea assente o lieve e assenza di sanguinamento attivo.


### 2

Criterio di dimissione dalla sala di risveglio raggiunto (≥ 9)

Confermare anche dolore controllato, nausea assente o lieve e assenza di sanguinamento attivo.


### 3

Al di sotto di 9: mantenere nella sala di risveglio

Rivalutare ogni 15 minuti e trattare ciò che impedisce la dimissione (dolore, ipossiemia, instabilità, sedazione residua).

