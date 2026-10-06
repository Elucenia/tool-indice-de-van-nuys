<!-- ELUCENIA technical documentation · indice-de-van-nuys · de · no clinical/professional/rights approval -->

# Van-Nuys-Prognoseindex (USC/VNPI)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/indice-de-van-nuys)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Größe des DCIS

`tam`

- `1` — ≤ 15 mm
- `2` — 16 bis 40 mm
- `3` — ≥ 41 mm

### Kleinster tumorfreier Resektionsrand

`margem`

- `1` — ≥ 10 mm
- `2` — 1 bis 9 mm
- `3` — \< 1 mm

### Pathologische Klassifikation

`pato`

- `1` — Nicht hochgradig, ohne Nekrose
- `2` — Nicht hochgradig, mit Nekrose
- `3` — Hochgradig (mit oder ohne Nekrose)

### Alter

`idade`

- `1` — \> 60 Jahre
- `2` — 40 bis 60 Jahre
- `3` — \< 40 Jahre

## Fassung der Methode

USC/VNPI/Silverstein 2003: 4 Faktoren mit Alter, gesamt 4–12; kein 3-Faktor-VNPI

## Dokumentierte Formel

Summe von 4 Faktoren, je 1–3: Größe, kleinster Rand, Pathologie (Kerngrad, Komedonekrose), Alter. Gesamt 4–12.

## Grenzen und Population

USC/VNPI 2003 wurde bei reinem DCIS nach brusterhaltender Operation untersucht und ergänzt die früheren drei Faktoren um das Alter. Er ist nicht der ursprüngliche Drei-Faktoren-Index und darf nicht automatisch auf invasives Karzinom angewendet werden. Behandlungsvorschläge spiegeln die beschriebene Grundlage wider und benötigen klinische Beurteilung und aktuelle Evidenz.

## Referenzen

- [Silverstein MJ. The University of Southern California/Van Nuys prognostic index for ductal carcinoma in situ of the breast. Am J Surg, 2003.](https://doi.org/10.1016/S0002-9610(03)00265-4)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

4 bis 6: alleinige Exzision erwägen

In der Serie von Silverstein veränderte die Strahlentherapie in dieser Gruppe das lokale rezidivfreie Überleben nach 12 Jahren nicht.


### 2

7 bis 9: Exzision mit Strahlentherapie (oder Re-Exzision, wenn der Rand < 10 mm ist)

Die Strahlentherapie brachte einen durchschnittlichen Gewinn von 12 bis 15% beim lokalen rezidivfreien Überleben.


### 3

10 bis 12: Mastektomie erwägen

Lokales Rezidiv von fast 50% nach 5 Jahren bei brusterhaltender Operation, auch mit Strahlentherapie; Re-Exzision nur, wenn technisch möglich.


### 4

10 bis 12: Mastektomie erwägen

Lokales Rezidiv von fast 50% nach 5 Jahren bei brusterhaltender Operation, auch mit Strahlentherapie; Re-Exzision nur, wenn technisch möglich.

