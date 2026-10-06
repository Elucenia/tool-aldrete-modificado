<!-- ELUCENIA technical documentation · aldrete-modificado · pt-BR · no clinical/professional/rights approval -->

# Índice de Aldrete modificado

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/aldrete-modificado)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Atividade motora

`atividade`

- `0` — Não move
- `1` — Move 2 membros
- `2` — Move os 4 membros

### Respiração

`resp`

- `0` — Apneia
- `1` — Dispneia ou respiração limitada
- `2` — Respira fundo e tosse

### Circulação (PA em relação à pré-anestésica)

`circ`

- `0` — Variação ≥ 50%
- `1` — Variação de 20 a 49%
- `2` — Variação ≤ 20%

### Consciência

`consc`

- `0` — Não responde
- `1` — Desperta ao ser chamado
- `2` — Totalmente desperto

### Saturação de O₂

`spo2`

- `0` — \< 90% mesmo com O₂
- `1` — Precisa de O₂ para manter \> 90%
- `2` — \> 92% em ar ambiente

## Edição do método

Modified Aldrete 1995:5 itens 0–2, Sp O 2 substituicor, total 0–10

## Fórmula documentada

Cinco itens de 0 a 2 pontos (total 0 a 10): atividade, respiração, circulação, consciência e saturação de O₂. A versão de 1995 trocou a cor da pele pela oximetria de pulso.

## Limites e população

Esta interface soma os cinco componentes do Aldrete modificado de recuperação pós-anestésica, com total de 0 a 10; não implementa o instrumento ambulatorial ampliado de dez fatores. O total isolado não autoriza alta e deve ser acompanhado de avaliação e reavaliação clínica. As tabelas originais de 1995 e a adaptação do autor de 2007 diferem na redação dos limites circulatórios; exatamente 20% permanece ambíguo. As tabelas de 1995 também divergem na última pontuação de oxigenação. Essas diferenças precisam de adjudicação clínica e não permitem afirmar equivalência integral apenas pela soma.

## Referências

- [Aldrete JA. The post-anesthesia recovery score revisited. J Clin Anesth, 1995.](https://doi.org/10.1016/0952-8180(94)00001-K)

- [Aldrete JA, Kroulik D. A postanesthetic recovery score. Anesth Analg, 1970.](https://doi.org/10.1213/00000539-197011000-00020)

- [JAntonioAldrete2007,RAA65(3),pp194–195](https://www.anestesia.org.ar/search/articulos_completos/1/1/1121/c.pdf)

- [Aldrete1995,originalletter,reproducedmirror](https://anest-rean.ru/wp-content/uploads/2024/11/Aldrete-J.A.-The-post-anesthesia-recovery-score-revisited.1995.pdf)

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

Critério de alta da sala de recuperação atingido (≥ 9)

Confirme também dor controlada, náusea ausente ou leve e ausência de sangramento ativo.


### 2

Critério de alta da sala de recuperação atingido (≥ 9)

Confirme também dor controlada, náusea ausente ou leve e ausência de sangramento ativo.


### 3

Abaixo de 9: manter na sala de recuperação

Reavalie a cada 15 minutos e trate o que impede a alta (dor, hipoxemia, instabilidade, sedação residual).

