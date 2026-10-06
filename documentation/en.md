<!-- ELUCENIA technical documentation · aldrete-modificado · en · no clinical/professional/rights approval -->

# Modified Aldrete score

[conditions, sources and permissions](https://elucenia.org/en/tools/aldrete-modificado)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Motor activity

`atividade`

- `0` — No movement
- `1` — Moves 2 limbs
- `2` — Moves all 4 limbs

### Breathing

`resp`

- `0` — Apnea
- `1` — Dyspnea or limited breathing
- `2` — Breathes deeply and coughs

### Circulation (blood pressure relative to preanesthetic baseline)

`circ`

- `0` — Variation ≥ 50%
- `1` — Variation of 20 to 49%
- `2` — Variation ≤ 20%

### Consciousness

`consc`

- `0` — Unresponsive
- `1` — Awakens to voice
- `2` — Fully awake

### O₂ saturation

`spo2`

- `0` — \< 90% even with O₂
- `1` — Needs O₂ to maintain \> 90%
- `2` — \> 92% on room air

## Method edition

Modified Aldrete 1995: 5 items 0–2, SpO₂ replaces colour, total 0–10

## Documented formula

Five items scored 0–2 (total 0–10): activity, respiration, circulation, consciousness and O₂ saturation. The 1995 version replaced skin colour with pulse oximetry.

## Limits and population

This interface sums the five components of the modified Aldrete for post-anesthesia recovery, with a total from 0 to 10; it does not implement the expanded ten-factor ambulatory instrument. The total alone does not authorize discharge and must be accompanied by clinical assessment and reassessment. The original 1995 tables and the author’s 2007 adaptation differ in the wording of the circulatory boundaries; exactly 20% remains ambiguous. The 1995 tables also differ in the lowest oxygenation score. These differences require clinical adjudication and do not allow complete equivalence to be claimed solely from the sum.

## References

- [Aldrete JA. The post-anesthesia recovery score revisited. J Clin Anesth, 1995.](https://doi.org/10.1016/0952-8180(94)00001-K)

- [Aldrete JA, Kroulik D. A postanesthetic recovery score. Anesth Analg, 1970.](https://doi.org/10.1213/00000539-197011000-00020)

- [JAntonioAldrete2007,RAA65(3),pp194–195](https://www.anestesia.org.ar/search/articulos_completos/1/1/1121/c.pdf)

- [Aldrete1995,originalletter,reproducedmirror](https://anest-rean.ru/wp-content/uploads/2024/11/Aldrete-J.A.-The-post-anesthesia-recovery-score-revisited.1995.pdf)

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

Recovery room discharge criterion reached (≥ 9)

Also confirm controlled pain, absent or mild nausea, and absence of active bleeding.


### 2

Recovery room discharge criterion reached (≥ 9)

Also confirm controlled pain, absent or mild nausea, and absence of active bleeding.


### 3

Below 9: keep in the recovery room

Reassess every 15 minutes and treat what prevents discharge (pain, hypoxemia, instability, residual sedation).

