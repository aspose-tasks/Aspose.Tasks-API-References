---
title: "PageLegend"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Seitenlegende dar, die für den Projekt‑Druck verwendet wird."
type: docs
weight: 177
url: /de/java/com.aspose.tasks/pagelegend/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.HeaderFooterInfo](../../com.aspose/tasks/headerfooterinfo)
```
public class PageLegend extends HeaderFooterInfo
```

Stellt eine Seitenlegende dar, die für den Projekt‑Druck verwendet wird.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PageLegend()](#PageLegend--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getLegendOn()](#getLegendOn--) | Ruft die Seiten ab, auf denen die Legende erscheint. |
| [getWidth()](#getWidth--) | Ruft die Breite des linken Teils (standardmäßig mit Projektname und Datum) der Legende in Zentimetern ab. |
| [setLegendOn(int value)](#setLegendOn-int-) | Setzt die Seiten, auf denen die Legende erscheint. |
| [setWidth(double value)](#setWidth-double-) | Setzt die Breite des linken Teils (standardmäßig mit Projektname und Datum) der Legende in Zentimetern. |
### PageLegend() {#PageLegend--}
```
public PageLegend()
```


### getLegendOn() {#getLegendOn--}
```
public final int getLegendOn()
```


Ruft die Seiten ab, auf denen die Legende erscheint. Kann einer der Werte der [Legend](../../com.aspose/tasks/legend)-Aufzählung sein.

**Returns:**
int – die Seiten, auf denen die Legende erscheint.
### getWidth() {#getWidth--}
```
public final double getWidth()
```


Ruft die Breite des linken Teils (standardmäßig mit Projektname und Datum) der Legende in Zentimetern ab.

**Returns:**
double – die Breite des linken Teils (standardmäßig mit Projektname und Datum) der Legende in Zentimetern.
### setLegendOn(int value) {#setLegendOn-int-}
```
public final void setLegendOn(int value)
```


Legt die Seiten fest, auf denen die Legende erscheint. Kann einer der Werte der [Legend](../../com.aspose.tasks/legend)-Aufzählung sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die Seiten, auf denen die Legende erscheint. |

### setWidth(double value) {#setWidth-double-}
```
public final void setWidth(double value)
```


Setzt die Breite des linken Teils (standardmäßig mit Projektname und Datum) der Legende in Zentimetern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | die Breite des linken Teils (enthält standardmäßig den Namen und das Datum des Projekts) der Legende in Zentimetern. |

