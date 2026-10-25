---
title: "GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt ein grafisches Indikator‑Kriterium dar, das mit einem erweiterten Attribut verknüpft ist."
type: docs
weight: 115
url: /de/java/com.aspose.tasks/graphicalindicatorcriteria/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteria
```

Stellt ein grafisches Indikator‑Kriterium dar, das mit einem erweiterten Attribut verknüpft ist.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Initialisiert eine neue Instanz des Typs [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria). |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Initialisiert eine neue Instanz des Typs [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getImageIndex()](#getImageIndex--) | Liefert den Index des Bildes, das angezeigt wird, wenn das Feld die Kriterien erfüllt. |
| [getRowType()](#getRowType--) | Liefert den Wert des Enums [GraphicalIndicatorCriteriaType](../../com.aspose/tasks/graphicalindicatorcriteriatype), das angibt, für welche Zeilen der Indikator angewendet wird. |
| [getTest()](#getTest--) | Liefert den Vergleichstyp, der zwischen dem Wert des erweiterten Attributs und den Werten durchgeführt wird und als Kriterium für die Anwendung des grafischen Indikators dient. |
| [getValue1()](#getValue1--) | Liefert den Wert, der zum Testen des Wertes des erweiterten Attributs verwendet wird. |
| [getValue2()](#getValue2--) | Liefert den zweiten Wert, der zum Testen des Wertes des erweiterten Attributs verwendet wird, falls die Vergleichstypen 'IsWithin' und 'IsNotWithin' vorliegen. |
| [toString()](#toString--) | Gibt die Zeichenkettenrepräsentation der Instanz der Klasse [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria) zurück. |
### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)
```


Initialisiert eine neue Instanz des Typs [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowType | int | Wert des Enums [GraphicalIndicatorCriteriaType](../../com.aspose/tasks/graphicalindicatorcriteriatype), das angibt, für welche Zeilen der Indikator angewendet wird |
| test | int | Wert von [FilterComparisonType](../../com.aspose/tasks/filtercomparisontype), der den von den Kriterien durchgeführten Vergleichstyp bezeichnet. |
| imageIndex | int | der Index des Bildes, das angezeigt wird, wenn das Feld die Kriterien erfüllt |
| value1 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | Werte, die bei der Bedingungsprüfung verwendet werden. |
| value2 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | zweiter Wert (Ende des Intervalls), der bei der Bedingungsprüfung im Fall von 'IsWithin' und 'IsNotWithing' Bedingungen verwendet wird. |

### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```


Initialisiert eine neue Instanz des Typs [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowType | int | Wert des Enums [GraphicalIndicatorCriteriaType](../../com.aspose/tasks/graphicalindicatorcriteriatype), das angibt, für welche Zeilen der Indikator angewendet wird |
| test | int | Wert von [FilterComparisonType](../../com.aspose/tasks/filtercomparisontype), der den von den Kriterien durchgeführten Vergleichstyp bezeichnet. |
| imageIndex | int | der Index des Bildes, das angezeigt wird, wenn das Feld die Kriterien erfüllt |
| value | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | Wert, der bei der Bedingungsprüfung verwendet wird. |

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Liefert den Index des Bildes, das angezeigt wird, wenn das Feld die Kriterien erfüllt.

**Returns:**
int - der Index des Bildes, das angezeigt wird, wenn das Feld die Kriterien erfüllt.
### getRowType() {#getRowType--}
```
public final int getRowType()
```


Liefert den Wert des Enums [GraphicalIndicatorCriteriaType](../../com.aspose/tasks/graphicalindicatorcriteriatype), das angibt, für welche Zeilen der Indikator angewendet wird.

**Returns:**
int - der Wert des Enums [GraphicalIndicatorCriteriaType](../../com.aspose/tasks/graphicalindicatorcriteriatype), das angibt, für welche Zeilen der Indikator angewendet wird.
### getTest() {#getTest--}
```
public final int getTest()
```


Liefert den Vergleichstyp, der zwischen dem Wert des erweiterten Attributs und den Werten durchgeführt wird und als Kriterium für die Anwendung des grafischen Indikators dient. [FilterComparisonType](../../com.aspose/tasks/filtercomparisontype)

**Returns:**
int - der Vergleichstyp, der zwischen dem Wert des erweiterten Attributs und den Werten durchgeführt wird und als Kriterium für die Anwendung des grafischen Indikators dient.
### getValue1() {#getValue1--}
```
public final GraphicalIndicatorCriteriaValue getValue1()
```


Liefert den Wert, der zum Testen des Wertes des erweiterten Attributs verwendet wird.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the value used to test extended attribute's value.
### getValue2() {#getValue2--}
```
public final GraphicalIndicatorCriteriaValue getValue2()
```


Liefert den zweiten Wert, der zum Testen des Wertes des erweiterten Attributs verwendet wird, falls die Vergleichstypen 'IsWithin' und 'IsNotWithin' vorliegen.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types.
### toString() {#toString--}
```
public String toString()
```


Gibt die Zeichenkettenrepräsentation der Instanz der Klasse [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria) zurück.

**Returns:**
java.lang.String - Zeichenkettenrepräsentation dieses Objekts.
