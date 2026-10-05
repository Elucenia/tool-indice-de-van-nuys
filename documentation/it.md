<!-- ELUCENIA technical documentation · indice-de-van-nuys · it · no clinical/professional/rights approval -->

# Indice prognostico di Van Nuys (USC/VNPI)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/indice-de-van-nuys)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Dimensione del carcinoma duttale in situ

`tam`

- `1` — ≤ 15 mm
- `2` — 16 a 40 mm
- `3` — ≥ 41 mm

### Margine libero minimo

`margem`

- `1` — ≥ 10 mm
- `2` — 1 a 9 mm
- `3` — \< 1 mm

### Classificazione patologica

`pato`

- `1` — Non di alto grado, senza necrosi
- `2` — Non di alto grado, con necrosi
- `3` — Alto grado (con o senza necrosi)

### Età

`idade`

- `1` — \> 60 anni
- `2` — 40 a 60 anni
- `3` — \< 40 anni

## Edizione del metodo

USC/VNPI/Silverstein 2003: 4 fattori con età, totale 4–12; non VNPI a 3 fattori

## Formula documentata

Somma di 4 fattori, ciascuno 1–3: dimensione, margine minimo, patologia (grado nucleare, necrosi comedonica), età. Totale 4–12.

## Limiti e popolazione

L’USC/VNPI 2003 è stato studiato nel CDIS puro trattato con chirurgia conservativa e aggiunge l’età ai tre fattori precedenti. Non è l’indice originale a tre fattori e non deve essere applicato automaticamente al carcinoma invasivo. I suggerimenti terapeutici riflettono la base descritta e richiedono una valutazione clinica ed evidenze contemporanee.

## Riferimenti

- [Silverstein MJ. The University of Southern California/Van Nuys prognostic index for ductal carcinoma in situ of the breast. Am J Surg, 2003.](https://doi.org/10.1016/S0002-9610(03)00265-4)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
