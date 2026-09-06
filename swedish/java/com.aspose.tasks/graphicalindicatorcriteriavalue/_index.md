---
title: "GraphicalIndicatorCriteriaValue"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar ett värde som används i villkorskontrollen för grafiska indikatorer."
type: docs
weight: 117
url: /sv/java/com.aspose.tasks/graphicalindicatorcriteriavalue/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteriaValue
```

Representerar ett värde som används i villkorskontrollen för grafiska indikatorer.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [GraphicalIndicatorCriteriaValue(BigDecimal value)](#GraphicalIndicatorCriteriaValue-java.math.BigDecimal-) | Skapar en instans av klassen GraphicalIndicatorCriteriaValue med ett konstant BigDecimal‑värde. |
| [GraphicalIndicatorCriteriaValue(Date dateValue)](#GraphicalIndicatorCriteriaValue-java.util.Date-) | Skapar en instans av klassen GraphicalIndicatorCriteriaValue med ett konstant datumvärde. |
| [GraphicalIndicatorCriteriaValue(String textValue)](#GraphicalIndicatorCriteriaValue-java.lang.String-) | Skapar en instans av klassen GraphicalIndicatorCriteriaValue med ett konstant strängvärde. |
| [GraphicalIndicatorCriteriaValue(Duration durationValue)](#GraphicalIndicatorCriteriaValue-com.aspose.tasks.Duration-) | Skapar en instans av klassen GraphicalIndicatorCriteriaValue med ett konstant varaktighetsvärde. |
| [GraphicalIndicatorCriteriaValue(boolean flagValue)](#GraphicalIndicatorCriteriaValue-boolean-) | Skapar en instans av klassen GraphicalIndicatorCriteriaValue med ett konstant flagg‑ (boolean)‑värde. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [createFieldLink(int field)](#createFieldLink-int-) | Skapar en instans av klassen GraphicalIndicatorCriteriaValue som representerar värdet för det angivna fältet i MS Project. |
| [getRawValue()](#getRawValue--) | Hämtar den underliggande konstanten för fältvärdet. |
| [isFieldLink()](#isFieldLink--) | Hämtar om den aktuella instansen är en fältlänk (representerar ett fältvärde). |
| [toString()](#toString--) | Returnerar en sträng som representerar det aktuella objektet. |
### GraphicalIndicatorCriteriaValue(BigDecimal value) {#GraphicalIndicatorCriteriaValue-java.math.BigDecimal-}
```
public GraphicalIndicatorCriteriaValue(BigDecimal value)
```


Skapar en instans av klassen GraphicalIndicatorCriteriaValue med ett konstant BigDecimal‑värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | det BigDecimal-värdet |

### GraphicalIndicatorCriteriaValue(Date dateValue) {#GraphicalIndicatorCriteriaValue-java.util.Date-}
```
public GraphicalIndicatorCriteriaValue(Date dateValue)
```


Skapar en instans av klassen GraphicalIndicatorCriteriaValue med ett konstant datumvärde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dateValue | java.util.Date | det Date-värdet |

### GraphicalIndicatorCriteriaValue(String textValue) {#GraphicalIndicatorCriteriaValue-java.lang.String-}
```
public GraphicalIndicatorCriteriaValue(String textValue)
```


Skapar en instans av klassen GraphicalIndicatorCriteriaValue med ett konstant strängvärde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| textValue | java.lang.String | det String-värdet |

### GraphicalIndicatorCriteriaValue(Duration durationValue) {#GraphicalIndicatorCriteriaValue-com.aspose.tasks.Duration-}
```
public GraphicalIndicatorCriteriaValue(Duration durationValue)
```


Skapar en instans av klassen GraphicalIndicatorCriteriaValue med ett konstant varaktighetsvärde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| durationValue | [Duration](../../com.aspose.tasks/duration) | det Duration-värdet |

### GraphicalIndicatorCriteriaValue(boolean flagValue) {#GraphicalIndicatorCriteriaValue-boolean-}
```
public GraphicalIndicatorCriteriaValue(boolean flagValue)
```


Skapar en instans av klassen GraphicalIndicatorCriteriaValue med ett konstant flagg‑ (boolean)‑värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| flagValue | boolean | flag-värdet (boolean) |

### createFieldLink(int field) {#createFieldLink-int-}
```
public static GraphicalIndicatorCriteriaValue createFieldLink(int field)
```


Skapar en instans av klassen GraphicalIndicatorCriteriaValue som representerar värdet för det angivna fältet i MS Project.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fält | int | det angivna fältet |

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - instance of GraphicalIndicatorCriteriaValue class representing the value of the specified field
### getRawValue() {#getRawValue--}
```
public final Object getRawValue()
```


Hämtar den underliggande konstanten för fältvärdet.

**Returns:**
java.lang.Object - det underliggande konstantvärdet för Field-värdet
### isFieldLink() {#isFieldLink--}
```
public final boolean isFieldLink()
```


Hämtar om den aktuella instansen är en fältlänk (representerar ett fältvärde).

**Returns:**
boolean - huruvida den aktuella instansen är en fältlänk (representerar ett värde av ett fält)
### toString() {#toString--}
```
public String toString()
```


Returnerar en sträng som representerar det aktuella objektet.

**Returns:**
java.lang.String - en sträng som representerar det aktuella objektet
