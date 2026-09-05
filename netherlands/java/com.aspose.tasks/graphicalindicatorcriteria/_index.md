---
title: "GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt één grafische indicatorcriterium voor dat is gekoppeld aan een uitgebreid attribuut."
type: docs
weight: 115
url: /nl/java/com.aspose.tasks/graphicalindicatorcriteria/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteria
```

Stelt één grafische indicatorcriterium voor dat is gekoppeld aan een uitgebreid attribuut.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Initialiseert een nieuw exemplaar van het type [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria). |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Initialiseert een nieuw exemplaar van het type [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria). |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getImageIndex()](#getImageIndex--) | Haalt de index op van de afbeelding die moet worden weergegeven wanneer het veld aan de criteria voldoet. |
| [getRowType()](#getRowType--) | Haalt de waarde op van de enum [GraphicalIndicatorCriteriaType](../../com.aspose/tasks/graphicalindicatorcriteriatype) die aangeeft op welke rijen de indicator wordt toegepast. |
| [getTest()](#getTest--) | Haalt het type vergelijking op dat wordt gemaakt tussen de waarde van het uitgebreide attribuut en waarden die dienen als criterium voor de toepassing van de grafische indicator. |
| [getValue1()](#getValue1--) | Haalt de waarde op die wordt gebruikt om de waarde van het uitgebreide attribuut te testen. |
| [getValue2()](#getValue2--) | Haalt de tweede waarde op die wordt gebruikt om de waarde van het uitgebreide attribuut te testen in het geval van de vergelijkingssoorten 'IsWithin' en 'IsNotWithin'. |
| [toString()](#toString--) | Retourneert de tekenreeksrepresentatie van de instantie van de klasse [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria). |
### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)
```


Initialiseert een nieuw exemplaar van het type [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| rowType | int | waarde van de enum [GraphicalIndicatorCriteriaType](../../com.aspose/tasks/graphicalindicatorcriteriatype) die aangeeft op welke rijen de indicator wordt toegepast |
| test | int | waarde van [FilterComparisonType](../../com.aspose/tasks/filtercomparisontype) die het type vergelijking aangeeft dat door het criterium wordt uitgevoerd. |
| imageIndex | int | de index van de afbeelding die moet worden weergegeven wanneer het veld aan de criteria voldoet |
| value1 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | waarden gebruikt bij de voorwaardelijke controle. |
| value2 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | tweede waarde (einde van interval) gebruikt bij de voorwaardelijke controle in het geval van 'IsWithin' en 'IsNotWithing' voorwaarden. |

### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```


Initialiseert een nieuw exemplaar van het type [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| rowType | int | waarde van de enum [GraphicalIndicatorCriteriaType](../../com.aspose/tasks/graphicalindicatorcriteriatype) die aangeeft op welke rijen de indicator wordt toegepast |
| test | int | waarde van [FilterComparisonType](../../com.aspose/tasks/filtercomparisontype) die het type vergelijking aangeeft dat door het criterium wordt uitgevoerd. |
| imageIndex | int | de index van de afbeelding die moet worden weergegeven wanneer het veld aan de criteria voldoet |
| value | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | waarde gebruikt bij de voorwaardelijke controle. |

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Haalt de index op van de afbeelding die moet worden weergegeven wanneer het veld aan de criteria voldoet.

**Returns:**
int - de index van de afbeelding die moet worden weergegeven wanneer het veld aan de criteria voldoet.
### getRowType() {#getRowType--}
```
public final int getRowType()
```


Haalt de waarde op van de enum [GraphicalIndicatorCriteriaType](../../com.aspose/tasks/graphicalindicatorcriteriatype) die aangeeft op welke rijen de indicator wordt toegepast.

**Returns:**
int - de waarde van de enum [GraphicalIndicatorCriteriaType](../../com.aspose/tasks/graphicalindicatorcriteriatype) die aangeeft op welke rijen de indicator wordt toegepast.
### getTest() {#getTest--}
```
public final int getTest()
```


Haalt het type vergelijking op dat wordt gemaakt tussen de waarde van het uitgebreide attribuut en waarden die dienen als criterium voor de toepassing van de grafische indicator. [FilterComparisonType](../../com.aspose/tasks/filtercomparisontype)

**Returns:**
int - het type vergelijking dat wordt gemaakt tussen de waarde van het uitgebreide attribuut en waarden die dienen als criterium voor de toepassing van de grafische indicator.
### getValue1() {#getValue1--}
```
public final GraphicalIndicatorCriteriaValue getValue1()
```


Haalt de waarde op die wordt gebruikt om de waarde van het uitgebreide attribuut te testen.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the value used to test extended attribute's value.
### getValue2() {#getValue2--}
```
public final GraphicalIndicatorCriteriaValue getValue2()
```


Haalt de tweede waarde op die wordt gebruikt om de waarde van het uitgebreide attribuut te testen in het geval van de vergelijkingssoorten 'IsWithin' en 'IsNotWithin'.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types.
### toString() {#toString--}
```
public String toString()
```


Retourneert de tekenreeksrepresentatie van de instantie van de klasse [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria).

**Returns:**
java.lang.String - tekenreeksrepresentatie van dit object.
