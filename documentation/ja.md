<!-- ELUCENIA technical documentation · aldrete-modificado · ja · no clinical/professional/rights approval -->

# 修正Aldreteスコア

[条件・出典・許諾](https://elucenia.org/ja/tools/aldrete-modificado)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 運動機能

`atividade`

- `0` — 動かさない
- `1` — 2肢を動かす
- `2` — 4肢すべてを動かす

### 呼吸

`resp`

- `0` — 無呼吸
- `1` — 呼吸困難または呼吸が制限される
- `2` — 深呼吸と咳ができる

### 循環（麻酔前と比較した血圧）

`circ`

- `0` — 変動≥50%
- `1` — 変動20～49%
- `2` — 変動≤20%

### 意識

`consc`

- `0` — 応答しない
- `1` — 呼びかけで覚醒
- `2` — 完全に覚醒

### 酸素飽和度

`spo2`

- `0` — O₂投与中でも\<90%
- `1` — \>90%を維持するためO₂が必要
- `2` — 室内気で\>92%

## 方法の版

改良Aldrete 1995：5項目0–2、SpO₂が皮膚色を代替、計0–10

## 記載された計算式

5項目各0–2点（計0–10）：活動、呼吸、循環、意識、O₂飽和度。1995年版では皮膚色をパルスオキシメトリに変更。

## 限界・対象集団

この画面は麻酔後回復の修正Aldreteの五つの要素を合計し、0～10点とします。外来手術用の十要素に拡張された評価は実装していません。合計点だけで退院を許可するものではなく、臨床評価と再評価を伴う必要があります。1995年の原表と著者による2007年の改編では循環指標の境界の表現が異なり、ちょうど20%はなお曖昧です。1995年の表同士でも酸素化の最後の点数が異なります。これらは臨床的な裁定が必要で、合計だけで完全な同等性を主張できません。

## 参考文献

- [Aldrete JA. The post-anesthesia recovery score revisited. J Clin Anesth, 1995.](https://doi.org/10.1016/0952-8180(94)00001-K)

- [Aldrete JA, Kroulik D. A postanesthetic recovery score. Anesth Analg, 1970.](https://doi.org/10.1213/00000539-197011000-00020)

- [JAntonioAldrete2007,RAA65(3),pp194–195](https://www.anestesia.org.ar/search/articulos_completos/1/1/1121/c.pdf)

- [Aldrete1995,originalletter,reproducedmirror](https://anest-rean.ru/wp-content/uploads/2024/11/Aldrete-J.A.-The-post-anesthesia-recovery-score-revisited.1995.pdf)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

回復室退室基準に到達（≥ 9）

痛みがコントロールされていること、悪心がないか軽度であること、活動性出血がないことも確認してください。


### 2

回復室退室基準に到達（≥ 9）

痛みがコントロールされていること、悪心がないか軽度であること、活動性出血がないことも確認してください。


### 3

9未満：回復室にとどめる

15分ごとに再評価し、退室を妨げる要因（疼痛、低酸素血症、不安定、残存鎮静）を治療する。

