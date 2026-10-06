<!-- ELUCENIA technical documentation · indice-de-van-nuys · es · no clinical/professional/rights approval -->

# Índice pronóstico de Van Nuys (USC/VNPI)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/indice-de-van-nuys)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Tamaño del CDIS

`tam`

- `1` — ≤ 15 mm
- `2` — 16 a 40 mm
- `3` — ≥ 41 mm

### Menor margen libre

`margem`

- `1` — ≥ 10 mm
- `2` — 1 a 9 mm
- `3` — \< 1 mm

### Clasificación patológica

`pato`

- `1` — No de alto grado, sin necrosis
- `2` — No de alto grado, con necrosis
- `3` — Alto grado (con o sin necrosis)

### Edad

`idade`

- `1` — \> 60 años
- `2` — 40 a 60 años
- `3` — \< 40 años

## Edición del método

USC/VNPI/Silverstein 2003: 4 factores con edad, total 4–12; no VNPI de 3 factores

## Fórmula documentada

Suma de 4 factores, cada uno 1–3: tamaño, menor margen, clasificación patológica (grado nuclear, necrosis comedo), edad. Total 4–12.

## Límites y población

El USC/VNPI 2003 se estudió en CDIS puro tratado con cirugía conservadora y añade la edad a los tres factores anteriores. No es el índice original de tres factores ni debe aplicarse automáticamente al carcinoma invasivo. Las sugerencias de tratamiento reflejan la base descrita y requieren evaluación clínica y evidencia contemporánea.

## Referencias

- [Silverstein MJ. The University of Southern California/Van Nuys prognostic index for ductal carcinoma in situ of the breast. Am J Surg, 2003.](https://doi.org/10.1016/S0002-9610(03)00265-4)

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

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

4 a 6: considerar exéresis sola

En la serie de Silverstein, la radioterapia no modificó la supervivencia libre de recidiva local a los 12 años en este grupo.


### 2

7 a 9: exéresis con radioterapia (o reexéresis si el margen es < 10 mm)

La radioterapia proporcionó una ganancia media de 12 a 15% en la supervivencia libre de recidiva local.


### 3

10 a 12: considerar mastectomía

Recidiva local de casi 50% a los 5 años con cirugía conservadora, incluso con radioterapia; reexéresis solo si es técnicamente posible.


### 4

10 a 12: considerar mastectomía

Recidiva local de casi 50% a los 5 años con cirugía conservadora, incluso con radioterapia; reexéresis solo si es técnicamente posible.

