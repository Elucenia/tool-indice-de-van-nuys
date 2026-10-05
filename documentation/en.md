<!-- ELUCENIA technical documentation · indice-de-van-nuys · en · no clinical/professional/rights approval -->

# Van Nuys Prognostic Index (USC/VNPI)

[conditions, sources and permissions](https://elucenia.org/en/tools/indice-de-van-nuys)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### DCIS size

`tam`

- `1` — ≤ 15 mm
- `2` — 16 to 40 mm
- `3` — ≥ 41 mm

### Smallest clear margin

`margem`

- `1` — ≥ 10 mm
- `2` — 1 to 9 mm
- `3` — \< 1 mm

### Pathological classification

`pato`

- `1` — Not high-grade, without necrosis
- `2` — Not high-grade, with necrosis
- `3` — High-grade (with or without necrosis)

### Age

`idade`

- `1` — \> 60 years
- `2` — 40 to 60 years
- `3` — \< 40 years

## Method edition

USC/VNPI/Silverstein 2003: 4 factors including age, total 4–12; not 3-factor VNPI

## Documented formula

Sum of 4 factors, each 1–3 points: size, closest margin, pathological classification (nuclear grade and comedo necrosis) and age. Total 4–12.

## Limits and population

USC/VNPI 2003 was studied in pure DCIS treated with breast-conserving surgery and adds age to the three previous factors. It is not the original three-factor index and must not be automatically applied to invasive carcinoma. Treatment suggestions reflect the described evidence base and require clinical assessment and contemporary evidence.

## References

- [Silverstein MJ. The University of Southern California/Van Nuys prognostic index for ductal carcinoma in situ of the breast. Am J Surg, 2003.](https://doi.org/10.1016/S0002-9610(03)00265-4)

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
