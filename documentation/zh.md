<!-- ELUCENIA technical documentation · aldrete-modificado · zh · no clinical/professional/rights approval -->

# 改良 Aldrete 评分

[条件、来源与许可](https://elucenia.org/zh/tools/aldrete-modificado)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 运动活动

`atividade`

- `0` — 不能活动
- `1` — 可活动2个肢体
- `2` — 可活动全部4个肢体

### 呼吸

`resp`

- `0` — 呼吸暂停
- `1` — 呼吸困难或呼吸受限
- `2` — 可深呼吸并咳嗽

### 循环（血压与麻醉前比较）

`circ`

- `0` — 变化≥50%
- `1` — 变化20至49%
- `2` — 变化≤20%

### 意识

`consc`

- `0` — 无应答
- `1` — 呼唤后苏醒
- `2` — 完全清醒

### 氧饱和度

`spo2`

- `0` — 即使吸O₂仍\<90%
- `1` — 需O₂才能维持\>90%
- `2` — 室内空气下\>92%

## 方法版本

改良Aldrete 1995：5项各0–2，SpO₂替代肤色，总分0–10

## 已记录的公式

五项各0–2分（总分0–10）：活动、呼吸、循环、意识、O₂饱和度。1995版用脉搏血氧替代肤色。

## 限制与适用人群

此界面汇总改良Aldrete麻醉后恢复的五个组成部分，总分0至10；未实现扩展的十因素门诊手术工具。总分不能单独批准出院，需结合临床评估及重复评估。1995年原始表格与作者2007年的改编在循环指标边界措辞上不同，恰好20%仍有歧义。1995年表格的最后一项氧合评分也不一致。这些差异需由临床人员裁定，仅凭求和不能宣称完全等同。

## 参考文献

- [Aldrete JA. The post-anesthesia recovery score revisited. J Clin Anesth, 1995.](https://doi.org/10.1016/0952-8180(94)00001-K)

- [Aldrete JA, Kroulik D. A postanesthetic recovery score. Anesth Analg, 1970.](https://doi.org/10.1213/00000539-197011000-00020)

- [JAntonioAldrete2007,RAA65(3),pp194–195](https://www.anestesia.org.ar/search/articulos_completos/1/1/1121/c.pdf)

- [Aldrete1995,originalletter,reproducedmirror](https://anest-rean.ru/wp-content/uploads/2024/11/Aldrete-J.A.-The-post-anesthesia-recovery-score-revisited.1995.pdf)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026
