<!-- ELUCENIA technical documentation · indice-de-van-nuys · pt-BR · no clinical/professional/rights approval -->

# Índice Prognóstico de Van Nuys (USC/VNPI)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/indice-de-van-nuys)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Tamanho do CDIS

`tam`

- `1` — ≤ 15 mm
- `2` — 16 a 40 mm
- `3` — ≥ 41 mm

### Menor margem livre

`margem`

- `1` — ≥ 10 mm
- `2` — 1 a 9 mm
- `3` — \< 1 mm

### Classificação patológica

`pato`

- `1` — Não alto grau, sem necrose
- `2` — Não alto grau, com necrose
- `3` — Alto grau (com ou sem necrose)

### Idade

`idade`

- `1` — \> 60 anos
- `2` — 40 a 60 anos
- `3` — \< 40 anos

## Edição do método

USC/VNPI/Silverstein 2003:4 fatores incluindoidade, total 4–12; sem VNPI 3 fatores

## Fórmula documentada

Soma de 4 fatores, cada um de 1 a 3 pontos: tamanho, menor margem, classificação patológica (grau nuclear e necrose comedo) e idade. Total de 4 a 12.

## Limites e população

O USC/VNPI 2003 foi estudado em CDIS puro tratado com cirurgia conservadora e acrescenta idade aos três fatores anteriores. Não é o índice original de três fatores nem deve ser aplicado automaticamente ao carcinoma invasivo. As sugestões de tratamento refletem a base descrita e exigem avaliação clínica e evidência contemporânea.

## Referências

- [Silverstein MJ. The University of Southern California/Van Nuys prognostic index for ductal carcinoma in situ of the breast. Am J Surg, 2003.](https://doi.org/10.1016/S0002-9610(03)00265-4)

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

4 a 6: considerar excisão isolada

Na série de Silverstein, a radioterapia não mudou a sobrevida livre de recidiva local em 12 anos neste grupo.


### 2

7 a 9: excisão com radioterapia (ou reexcisão se a margem for < 10 mm)

A radioterapia deu ganho médio de 12 a 15% na sobrevida livre de recidiva local.


### 3

10 a 12: considerar mastectomia

Recidiva local de quase 50% em 5 anos com cirurgia conservadora, mesmo com radioterapia; reexcisão só se tecnicamente possível.


### 4

10 a 12: considerar mastectomia

Recidiva local de quase 50% em 5 anos com cirurgia conservadora, mesmo com radioterapia; reexcisão só se tecnicamente possível.

