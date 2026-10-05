<!-- ELUCENIA technical documentation · aldrete-modificado · es · no clinical/professional/rights approval -->

# Índice de Aldrete modificado

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/aldrete-modificado)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Actividad motora

`atividade`

- `0` — No mueve
- `1` — Mueve 2 extremidades
- `2` — Mueve las 4 extremidades

### Respiración

`resp`

- `0` — Apnea
- `1` — Disnea o respiración limitada
- `2` — Respira profundamente y tose

### Circulación (presión arterial respecto a la preanestésica)

`circ`

- `0` — Variación ≥ 50%
- `1` — Variación del 20 al 49%
- `2` — Variación ≤ 20%

### Conciencia

`consc`

- `0` — No responde
- `1` — Despierta al llamarlo
- `2` — Completamente despierto

### Saturación de O₂

`spo2`

- `0` — \< 90% incluso con O₂
- `1` — Necesita O₂ para mantener \> 90%
- `2` — \> 92% en aire ambiente

## Edición del método

Aldrete modificado 1995: 5 ítems 0–2, SpO₂ reemplaza color, total 0–10

## Fórmula documentada

Cinco ítems de 0–2 puntos (total 0–10): actividad, respiración, circulación, conciencia y saturación O₂. La versión 1995 sustituyó el color de piel por pulsioximetría.

## Límites y población

Esta interfaz suma los cinco componentes del Aldrete modificado para la recuperación posanestésica, con un total de 0 a 10; no implementa el instrumento ambulatorio ampliado de diez factores. El total aislado no autoriza el alta y debe acompañarse de evaluación y reevaluación clínica. Las tablas originales de 1995 y la adaptación del autor de 2007 difieren en la redacción de los límites circulatorios; exactamente 20% sigue siendo ambiguo. Las tablas de 1995 también difieren en la puntuación más baja de oxigenación. Estas diferencias requieren adjudicación clínica y no permiten afirmar una equivalencia integral solo por la suma.

## Referencias

- [Aldrete JA. The post-anesthesia recovery score revisited. J Clin Anesth, 1995.](https://doi.org/10.1016/0952-8180(94)00001-K)

- [Aldrete JA, Kroulik D. A postanesthetic recovery score. Anesth Analg, 1970.](https://doi.org/10.1213/00000539-197011000-00020)

- [JAntonioAldrete2007,RAA65(3),pp194–195](https://www.anestesia.org.ar/search/articulos_completos/1/1/1121/c.pdf)

- [Aldrete1995,originalletter,reproducedmirror](https://anest-rean.ru/wp-content/uploads/2024/11/Aldrete-J.A.-The-post-anesthesia-recovery-score-revisited.1995.pdf)

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
