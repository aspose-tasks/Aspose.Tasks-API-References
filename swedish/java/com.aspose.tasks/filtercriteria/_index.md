---
title: "FilterCriteria"
second_title: "Aspose.Tasks for Java API-referens"
description: "Definierar kriterierna som uppgifter eller resurser måste uppfylla för att visas i MSP-vyn."
type: docs
weight: 94
url: /sv/java/com.aspose.tasks/filtercriteria/
---

**Inheritance:**
java.lang.Object
```
public class FilterCriteria
```

Definierar kriterierna som uppgifter eller resurser måste uppfylla för att visas i MSP-vyn.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [FilterCriteria()](#FilterCriteria--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCriteriaRows()](#getCriteriaRows--) | Hämtar listan över underordnade [FilterCriteria](../../com.aspose.tasks/filtercriteria) rader. |
| [getField()](#getField--) | Hämtar ett `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) för att ändra. |
| [getOperation()](#getOperation--) | Hämtar kriteriet som etablerats med FieldName, Test och Value och som relaterar till andra kriterier i filtret. |
| [getTest()](#getTest--) | Hämtar typen av jämförelse som görs mellan FieldName och Value och som fungerar som urvalskriterium för filtret. |
| [getValues()](#getValues--) | Hämtar objektvärdena för att jämföra med värdet på fältet som specificerats med FieldName. |
| [isValueAField()](#isValueAField--) | Hämtar om det högra värdet i FilterCriteria är en fältreferens, inte ett konstantvärde. |
| [isValueAField(int index)](#isValueAField-int-) | Hämtar om värdet på indexet i FilterCriteria är en fältreferens, inte ett konstantvärde. |
| [setField(int value)](#setField-int-) | Ställer in ett `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) för att ändra. |
| [setOperation(int value)](#setOperation-int-) | Ställer in kriteriet som etablerats med FieldName, Test och Value och som relaterar till andra kriterier i filtret. |
| [setTest(int value)](#setTest-int-) | Ställer in typen av jämförelse som görs mellan FieldName och Value och som fungerar som urvalskriterium för filtret. |
| [setValue(int index, Object value)](#setValue-int-java.lang.Object-) | Ställer in objektvärdet på indexet för att jämföra med värdet på fältet som specificerats av FieldName. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Ställer in objektvärdet för att jämföra med värdet på fältet som specificerats av FieldName. |
| [setValueByField(int value)](#setValueByField-int-) | Ställer in fältet vars värde kommer att jämföras med värdet på fältet som specificerats av FieldName. |
| [setValueByField(int index, int value)](#setValueByField-int-int-) | Ställer in fältet på indexet vars värde kommer att jämföras med värdet på fältet som specificerats av FieldName. |
| [toString()](#toString--) | Returnerar en strängrepresentation av instansen av klassen [FilterCriteria](../../com.aspose.tasks/filtercriteria). |
### FilterCriteria() {#FilterCriteria--}
```
public FilterCriteria()
```


### getCriteriaRows() {#getCriteriaRows--}
```
public final List<FilterCriteria> getCriteriaRows()
```


Hämtar listan över underordnade [FilterCriteria](../../com.aspose.tasks/filtercriteria) rader. Om filtret innehåller mer än en kriterierad rad är effekten av en And-operator att kriterierna för båda raderna måste uppfyllas för att uppgiften eller resursen ska visas som ett resultat av detta filter. Effekten av en Or-operator är att kriterierna för den ena eller den andra raden måste uppfyllas.

**Returns:**
java.util.List&lt;com.aspose.tasks.FilterCriteria&gt; - listan med underordnade [FilterCriteria](../../com.aspose.tasks/filtercriteria) rader.
### getField() {#getField--}
```
public final int getField()
```


Hämtar ett `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) för att ändra.

**Returns:**
int - ett `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) att ändra.
### getOperation() {#getOperation--}
```
public final int getOperation()
```


Hämtar kriteriet som etablerats med FieldName, Test och Value och som relaterar till andra kriterier i filtret.

**Returns:**
int - kriteriet som etableras med FieldName, Test och Value förhåller sig till andra kriterier i filtret.
### getTest() {#getTest--}
```
public final int getTest()
```


Hämtar typen av jämförelse som görs mellan FieldName och Value och som fungerar som urvalskriterium för filtret. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - typen av jämförelse som görs mellan FieldName och Value och som fungerar som urvalskriterium för filtret.
### getValues() {#getValues--}
```
public final Object[] getValues()
```


Hämtar objektvärdena för att jämföra med värdet på fältet som specificerats med FieldName.

**Returns:**
java.lang.Object[] - objektvärdena att jämföra med värdet på fältet som specificerats med FieldName.
### isValueAField() {#isValueAField--}
```
public final boolean isValueAField()
```


Hämtar om det högra värdet i FilterCriteria är en fältreferens, inte ett konstantvärde.

**Returns:**
boolean - om det högra värdet av FilterCriteria är en fältreferens, inte ett konstantvärde.
### isValueAField(int index) {#isValueAField-int-}
```
public final boolean isValueAField(int index)
```


Hämtar om värdet på indexet i FilterCriteria är en fältreferens, inte ett konstantvärde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | indexet för värdet |

**Returns:**
boolean - om det högra värdet vid indexet för FilterCriteria är en fältreferens, inte ett konstantvärde.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Ställer in ett `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) för att ändra.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | int | ett `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) att ändra. |

### setOperation(int value) {#setOperation-int-}
```
public final void setOperation(int value)
```


Ställer in kriteriet som etablerats med FieldName, Test och Value och som relaterar till andra kriterier i filtret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | kriteriet som etableras med FieldName, Test och Value förhåller sig till andra kriterier i filtret. |

### setTest(int value) {#setTest-int-}
```
public final void setTest(int value)
```


Ställer in typen av jämförelse som görs mellan FieldName och Value och som fungerar som urvalskriterium för filtret. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | typen av jämförelse som görs mellan FieldName och Value och som fungerar som urvalskriterium för filtret. |

### setValue(int index, Object value) {#setValue-int-java.lang.Object-}
```
public final void setValue(int index, Object value)
```


Ställer in objektvärdet på indexet för att jämföra med värdet på fältet som specificerats av FieldName.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | indexet för värdet. |
| värde | java.lang.Object | objektvärde som kommer att fungera som högra värde vid indexet för filterkriterier. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public final void setValue(Object value)
```


Ställer in objektvärdet för att jämföra med värdet på fältet som specificerats av FieldName.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object | objektvärde som kommer att fungera som högra värde för filterkriterier. |

### setValueByField(int value) {#setValueByField-int-}
```
public final void setValueByField(int value)
```


Ställer in fältet vars värde kommer att jämföras med värdet på fältet som specificerats av FieldName.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | Fält som kommer att fungera som högra värde för filterkriterier. |

### setValueByField(int index, int value) {#setValueByField-int-int-}
```
public final void setValueByField(int index, int value)
```


Ställer in fältet på indexet vars värde kommer att jämföras med värdet på fältet som specificerats av FieldName.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | indexet för värdet |
| värde | int | Fält som kommer att fungera som högra värde vid indexet för filterkriterier. |

### toString() {#toString--}
```
public String toString()
```


Returnerar en strängrepresentation av instansen av klassen [FilterCriteria](../../com.aspose.tasks/filtercriteria).

**Returns:**
java.lang.String - strängrepresentation av detta objekt.
