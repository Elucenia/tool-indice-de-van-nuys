<!-- ELUCENIA technical documentation · indice-de-van-nuys · ja · no clinical/professional/rights approval -->

# Van Nuys予後指数（USC/VNPI）

[条件・出典・許諾](https://elucenia.org/ja/tools/indice-de-van-nuys)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 非浸潤性乳管癌（DCIS）の大きさ

`tam`

- `1` — ≤ 15 mm
- `2` — 16 ～ 40 mm
- `3` — ≥ 41 mm

### 最小の陰性断端幅

`margem`

- `1` — ≥ 10 mm
- `2` — 1 ～ 9 mm
- `3` — \< 1 mm

### 病理分類

`pato`

- `1` — 高異型度でなく，壊死なし
- `2` — 高異型度でなく，壊死あり
- `3` — 高異型度（壊死の有無は問わない）

### 年齢

`idade`

- `1` — \> 60 歳
- `2` — 40 ～ 60 歳
- `3` — \< 40 歳

## 方法の版

USC/VNPI/Silverstein 2003：年齢を含む4因子、計4–12；3因子VNPIではない

## 記載された計算式

4因子各1–3点：径、最小断端幅、病理分類（核グレード・コメド壊死）、年齢。計4–12。

## 限界・対象集団

USC/VNPI 2003は、乳房温存手術で治療した純粋な非浸潤性乳管がん（DCIS）で研究され、従来の三因子に年齢を加えました。原来の三因子指数ではなく、浸潤がんへ自動的に適用してはいけません。治療の提案は記載された基盤を反映したもので、臨床評価と現代の証拠が必要です。

## 参考文献

- [Silverstein MJ. The University of Southern California/Van Nuys prognostic index for ductal carcinoma in situ of the breast. Am J Surg, 2003.](https://doi.org/10.1016/S0002-9610(03)00265-4)

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
