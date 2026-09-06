---
title: "GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar ett grafiskt indikatorvillkor som är associerat med ett utökat attribut."
type: docs
weight: 115
url: /sv/java/com.aspose.tasks/graphicalindicatorcriteria/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteria
```

Representerar ett grafiskt indikatorvillkor som är associerat med ett utökat attribut.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Initierar en ny instans av typen [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Initierar en ny instans av typen [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getImageIndex()](#getImageIndex--) | Hämtar indexet för bilden som ska visas när fältet uppfyller kriterierna. |
| [getRowType()](#getRowType--) | Hämtar värdet av enumen [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) som anger för vilka rader indikatorn tillämpas. |
| [getTest()](#getTest--) | Hämtar typen av jämförelse som görs mellan det utökade attributets värde och värden som fungerar som kriterium för tillämpningen av den grafiska indikatorn. |
| [getValue1()](#getValue1--) | Hämtar värdet som används för att testa det utökade attributets värde. |
| [getValue2()](#getValue2--) | Hämtar det andra värdet som används för att testa det utökade attributets värde i fall av jämförelsetyperna 'IsWithin' och 'IsNotWithin'. |
| [toString()](#toString--) | Returnerar en strängrepresentation av instansen av klassen [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)
```


Initierar en ny instans av typen [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowType | int | värde av enumen [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) som anger för vilka rader indikatorn tillämpas |
| test | int | värde av [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) som anger vilken typ av jämförelse som utförs av kriteriet. |
| imageIndex | int | indexet för bilden som ska visas när fältet uppfyller kriterierna |
| value1 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | värden som används i villkorskontrollen. |
| value2 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | andra värdet (slutet av intervallet) som används i villkorskontrollen i fall av 'IsWithin' och 'IsNotWithing'-villkor. |

### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```


Initierar en ny instans av typen [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowType | int | värde av enumen [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) som anger för vilka rader indikatorn tillämpas |
| test | int | värde av [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) som anger vilken typ av jämförelse som utförs av kriteriet. |
| imageIndex | int | indexet för bilden som ska visas när fältet uppfyller kriterierna |
| value | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | värde som används i villkorskontrollen. |

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Hämtar indexet för bilden som ska visas när fältet uppfyller kriterierna.

**Returns:**
int - indexet för bilden som ska visas när fältet uppfyller kriterierna.
### getRowType() {#getRowType--}
```
public final int getRowType()
```


Hämtar värdet av enumen [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) som anger för vilka rader indikatorn tillämpas.

**Returns:**
int - värdet av enumen [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) som anger för vilka rader indikatorn tillämpas.
### getTest() {#getTest--}
```
public final int getTest()
```


Hämtar typen av jämförelse som görs mellan det utökade attributets värde och värden som fungerar som kriterium för tillämpningen av den grafiska indikatorn. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - typen av jämförelse som görs mellan det utökade attributets värde och värden som fungerar som kriterium för tillämpningen av den grafiska indikatorn.
### getValue1() {#getValue1--}
```
public final GraphicalIndicatorCriteriaValue getValue1()
```


Hämtar värdet som används för att testa det utökade attributets värde.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the value used to test extended attribute's value.
### getValue2() {#getValue2--}
```
public final GraphicalIndicatorCriteriaValue getValue2()
```


Hämtar det andra värdet som används för att testa det utökade attributets värde i fall av jämförelsetyperna 'IsWithin' och 'IsNotWithin'.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types.
### toString() {#toString--}
```
public String toString()
```


Returnerar en strängrepresentation av instansen av klassen [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Returns:**
java.lang.String - strängrepresentation av detta objekt.
