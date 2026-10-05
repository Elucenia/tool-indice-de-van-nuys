<!-- ELUCENIA technical documentation · indice-de-van-nuys · zh · no clinical/professional/rights approval -->

# Van Nuys 预后指数（USC/VNPI）

[条件、来源与许可](https://elucenia.org/zh/tools/indice-de-van-nuys)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 导管原位癌（DCIS）大小

`tam`

- `1` — ≤ 15 mm
- `2` — 16 至 40 mm
- `3` — ≥ 41 mm

### 最小阴性切缘

`margem`

- `1` — ≥ 10 mm
- `2` — 1 至 9 mm
- `3` — \< 1 mm

### 病理分类

`pato`

- `1` — 非高级别，无坏死
- `2` — 非高级别，有坏死
- `3` — 高级别（有或无坏死）

### 年龄

`idade`

- `1` — \> 60 岁
- `2` — 40 至 60 岁
- `3` — \< 40 岁

## 方法版本

USC/VNPI/Silverstein 2003：4因素含年龄，总分4–12；非3因素VNPI

## 已记录的公式

4因素各1–3分相加：大小、最小切缘、病理分类（核分级、粉刺样坏死）、年龄。总分4–12。

## 限制与适用人群

USC/VNPI 2003在接受保乳手术的纯导管原位癌（DCIS）中研究，在此前三个因素上加入年龄。它不是原始三因素指数，也不应自动应用于浸润性癌。治疗建议反映所述证据基础，需要临床评估及当前证据支持。

## 参考文献

- [Silverstein MJ. The University of Southern California/Van Nuys prognostic index for ductal carcinoma in situ of the breast. Am J Surg, 2003.](https://doi.org/10.1016/S0002-9610(03)00265-4)

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
