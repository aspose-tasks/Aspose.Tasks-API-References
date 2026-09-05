---
title: "FilterCriteria"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Definieert de criteria waaraan taken of resources moeten voldoen om weergegeven te worden in de MSP-weergave."
type: docs
weight: 94
url: /nl/java/com.aspose.tasks/filtercriteria/
---

**Inheritance:**
java.lang.Object
```
public class FilterCriteria
```

Definieert de criteria waaraan taken of resources moeten voldoen om weergegeven te worden in de MSP-weergave.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [FilterCriteria()](#FilterCriteria--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCriteriaRows()](#getCriteriaRows--) | Haalt de lijst met onderliggende [FilterCriteria](../../com.aspose.tasks/filtercriteria) rijen op. |
| [getField()](#getField--) | Haalt een `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) op om te wijzigen. |
| [getOperation()](#getOperation--) | Haalt het criterium op dat is vastgesteld met FieldName, Test en Value en dat betrekking heeft op andere criteria in het filter. |
| [getTest()](#getTest--) | Haalt het type vergelijking op dat wordt gemaakt tussen FieldName en Value en dat dient als selectiecriterium voor het filter. |
| [getValues()](#getValues--) | Haalt de objectwaarden op om te vergelijken met de waarde van het veld dat is opgegeven met FieldName. |
| [isValueAField()](#isValueAField--) | Haalt op of de rechterwaarde van FilterCriteria een veldreferentie is, geen constante waarde. |
| [isValueAField(int index)](#isValueAField-int-) | Haalt op of de waarde op de index van FilterCriteria een veldreferentie is, geen constante waarde. |
| [setField(int value)](#setField-int-) | Stelt een `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) in om te wijzigen. |
| [setOperation(int value)](#setOperation-int-) | Stelt het criterium in dat is vastgesteld met FieldName, Test en Value en dat betrekking heeft op andere criteria in het filter. |
| [setTest(int value)](#setTest-int-) | Stelt het type vergelijking in dat wordt gemaakt tussen FieldName en Value en dat dient als selectiecriterium voor het filter. |
| [setValue(int index, Object value)](#setValue-int-java.lang.Object-) | Stelt de objectwaarde op de index in om te vergelijken met de waarde van het veld gespecificeerd door FieldName. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Stelt de objectwaarde in om te vergelijken met de waarde van het veld gespecificeerd door FieldName. |
| [setValueByField(int value)](#setValueByField-int-) | Stelt het veld in waarvan de waarde wordt vergeleken met de waarde van het veld gespecificeerd door FieldName. |
| [setValueByField(int index, int value)](#setValueByField-int-int-) | Stelt het veld op de index in waarvan de waarde wordt vergeleken met de waarde van het veld gespecificeerd door FieldName. |
| [toString()](#toString--) | Retourneert de tekenreeksrepresentatie van de instantie van de [FilterCriteria](../../com.aspose.tasks/filtercriteria) klasse. |
### FilterCriteria() {#FilterCriteria--}
```
public FilterCriteria()
```


### getCriteriaRows() {#getCriteriaRows--}
```
public final List<FilterCriteria> getCriteriaRows()
```


Haalt de lijst met onderliggende [FilterCriteria](../../com.aspose.tasks/filtercriteria) rijen op. Als het filter meer dan één criteriumrij bevat, is het effect van een AND-operator dat de criteria voor beide rijen moeten worden voldaan zodat de taak of bron als resultaat van dit filter wordt weergegeven. Het effect van een OR-operator is dat de criteria voor de ene of de andere rij moeten worden voldaan.

**Returns:**
java.util.List&lt;com.aspose.tasks.FilterCriteria&gt; - de lijst met onderliggende [FilterCriteria](../../com.aspose.tasks/filtercriteria) rijen.
### getField() {#getField--}
```
public final int getField()
```


Haalt een `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) op om te wijzigen.

**Returns:**
int - een `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) om te wijzigen.
### getOperation() {#getOperation--}
```
public final int getOperation()
```


Haalt het criterium op dat is vastgesteld met FieldName, Test en Value en dat betrekking heeft op andere criteria in het filter.

**Returns:**
int - het criterium vastgesteld met FieldName, Test en Value dat betrekking heeft op andere criteria in het filter.
### getTest() {#getTest--}
```
public final int getTest()
```


Haalt het type vergelijking op dat wordt gemaakt tussen FieldName en Value en dat dient als selectiecriterium voor het filter. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - het type vergelijking dat wordt gemaakt tussen FieldName en Value en dat dient als selectiecriterium voor het filter.
### getValues() {#getValues--}
```
public final Object[] getValues()
```


Haalt de objectwaarden op om te vergelijken met de waarde van het veld dat is opgegeven met FieldName.

**Returns:**
java.lang.Object[] - de objectwaarden om te vergelijken met de waarde van het veld gespecificeerd met FieldName.
### isValueAField() {#isValueAField--}
```
public final boolean isValueAField()
```


Haalt op of de rechterwaarde van FilterCriteria een veldreferentie is, geen constante waarde.

**Returns:**
boolean - of de rechterwaarde van FilterCriteria een veldreferentie is, geen constante waarde.
### isValueAField(int index) {#isValueAField-int-}
```
public final boolean isValueAField(int index)
```


Haalt op of de waarde op de index van FilterCriteria een veldreferentie is, geen constante waarde.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | de index van de waarde |

**Returns:**
boolean - of de rechterwaarde op de index van FilterCriteria een veldreferentie is, geen constante waarde.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Stelt een `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) in om te wijzigen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | int | een `Field`([getField()](../../com.aspose/tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) om te wijzigen. |

### setOperation(int value) {#setOperation-int-}
```
public final void setOperation(int value)
```


Stelt het criterium in dat is vastgesteld met FieldName, Test en Value en dat betrekking heeft op andere criteria in het filter.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het criterium vastgesteld met FieldName, Test en Value heeft betrekking op andere criteria in het filter. |

### setTest(int value) {#setTest-int-}
```
public final void setTest(int value)
```


Stelt het type vergelijking in dat wordt gemaakt tussen FieldName en Value en fungeert als selectiecriteria voor het filter. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het type vergelijking gemaakt tussen FieldName en Value dat fungeert als selectiecriteria voor het filter. |

### setValue(int index, Object value) {#setValue-int-java.lang.Object-}
```
public final void setValue(int index, Object value)
```


Stelt de objectwaarde op de index in om te vergelijken met de waarde van het veld gespecificeerd door FieldName.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | de index van de waarde. |
| waarde | java.lang.Object | objectwaarde die zal dienen als rechterwaarde op de index van filtercriteria. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public final void setValue(Object value)
```


Stelt de objectwaarde in om te vergelijken met de waarde van het veld gespecificeerd door FieldName.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.Object | objectwaarde die zal dienen als rechterwaarde van filtercriteria. |

### setValueByField(int value) {#setValueByField-int-}
```
public final void setValueByField(int value)
```


Stelt het veld in waarvan de waarde wordt vergeleken met de waarde van het veld gespecificeerd door FieldName.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | Veld dat zal dienen als rechterwaarde van filtercriteria. |

### setValueByField(int index, int value) {#setValueByField-int-int-}
```
public final void setValueByField(int index, int value)
```


Stelt het veld op de index in waarvan de waarde wordt vergeleken met de waarde van het veld gespecificeerd door FieldName.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | de index van de waarde |
| waarde | int | Veld dat zal dienen als rechterwaarde op de index van filtercriteria. |

### toString() {#toString--}
```
public String toString()
```


Retourneert de tekenreeksrepresentatie van de instantie van de [FilterCriteria](../../com.aspose.tasks/filtercriteria) klasse.

**Returns:**
java.lang.String - tekenreeksrepresentatie van dit object.
