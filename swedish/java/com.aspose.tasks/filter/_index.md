---
title: "Filter"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar ett filter i Project."
type: docs
weight: 91
url: /sv/java/com.aspose.tasks/filter/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public final class Filter implements Comparable<Filter>, System.IEquatable<Filter>
```

Representerar ett filter i Project.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Filter()](#Filter--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [compareTo(Filter other)](#compareTo-com.aspose.tasks.Filter-) | Jämför detta objekt med den angivna instansen av klassen [Filter](../../com.aspose.tasks/filter) och returnerar en indikation på deras relativa ordning. |
| [equals(Filter other)](#equals-com.aspose.tasks.Filter-) | Returnerar ett värde som indikerar om detta objekt är lika med det angivna AssignmentBaseline-objektet. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returnerar ett värde som indikerar om detta objekt är lika med det angivna AssignmentBaseline-objektet. |
| [getCriteria()](#getCriteria--) | Hämtar kriterierna som uppgifter eller resurser måste uppfylla för att visas i MSP-vyn. |
| [getFilterType()](#getFilterType--) | Hämtar filtretypen. |
| [getIndex()](#getIndex--) | Hämtar indexet för ett [Filter](../../com.aspose.tasks/filter)-objekt i det objekt som innehåller Filters. |
| [getName()](#getName--) | Hämtar namnet på ett Filter-objekt. |
| [getShowInMenu()](#getShowInMenu--) | Hämtar ett värde som anger om projektet visar filtreringsnamnet i Filter‑rullgardinslistan på fliken Visa i menyfliksområdet. |
| [getShowRelatedSummaryRows()](#getShowRelatedSummaryRows--) | Hämtar ett värde som anger om relaterade sammanfattningsrader visas för filtret. |
| [getUid()](#getUid--) | Hämtar den unika identifieraren för ett filter. |
| [hashCode()](#hashCode--) | Returnerar ett hash‑kodvärde för filtret. |
| [op_Equality(Filter a, Filter b)](#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [op_GreaterThan(Filter a, Filter b)](#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Returnerar ett värde som anger om detta objekt är större än ett angivet objekt. |
| [op_GreaterThanOrEqual(Filter a, Filter b)](#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Returnerar ett värde som anger om detta objekt är större än eller lika med ett angivet objekt. |
| [op_Inequality(Filter a, Filter b)](#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Returnerar ett värde som anger om detta objekt inte är lika med ett angivet objekt. |
| [op_LessThan(Filter a, Filter b)](#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Returnerar ett värde som anger om detta objekt är mindre än ett angivet objekt. |
| [op_LessThanOrEqual(Filter a, Filter b)](#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Returnerar ett värde som anger om detta objekt är mindre än eller lika med ett angivet objekt. |
| [setCriteria(FilterCriteria value)](#setCriteria-com.aspose.tasks.FilterCriteria-) | Ställer in kriterierna som uppgifter eller resurser måste uppfylla för att visas i MSP‑vyn. |
| [setFilterType(int value)](#setFilterType-int-) | Typen av filtret. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in namnet på ett Filter-objekt. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Ställer in ett värde som anger om projektet visar filtreringsnamnet i Filter‑rullgardinslistan på fliken Visa i menyfliksområdet. |
| [setShowRelatedSummaryRows(boolean value)](#setShowRelatedSummaryRows-boolean-) | Ställer in ett värde som anger om relaterade sammanfattningsrader visas för filtret. |
### Filter() {#Filter--}
```
public Filter()
```


### compareTo(Filter other) {#compareTo-com.aspose.tasks.Filter-}
```
public final int compareTo(Filter other)
```


Jämför detta objekt med den angivna instansen av klassen [Filter](../../com.aspose.tasks/filter) och returnerar en indikation på deras relativa ordning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | den angivna instansen av klassen [Filter](../../com.aspose.tasks/filter) att jämföra med detta objekt. |

**Returns:**
int – en indikation på deras relativa ordning.
### equals(Filter other) {#equals-com.aspose.tasks.Filter-}
```
public final boolean equals(Filter other)
```


Returnerar ett värde som indikerar om detta objekt är lika med det angivna AssignmentBaseline-objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | det angivna AssignmentBaseline-objektet att jämföra med denna instans. |

**Returns:**
boolean – returnerar true om denna instans är lika med det angivna AssignmentBaseline-objektet; annars false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returnerar ett värde som indikerar om detta objekt är lika med det angivna AssignmentBaseline-objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | det angivna AssignmentBaseline-objektet att jämföra med denna instans. |

**Returns:**
boolean – returnerar true om denna instans är lika med det angivna AssignmentBaseline-objektet; annars false.
### getCriteria() {#getCriteria--}
```
public final FilterCriteria getCriteria()
```


Hämtar kriterierna som uppgifter eller resurser måste uppfylla för att visas i MSP-vyn.

**Returns:**
[FilterCriteria](../../com.aspose.tasks/filtercriteria) - the criteria that tasks or resources must meet to be displayed in MSP view.
### getFilterType() {#getFilterType--}
```
public final int getFilterType()
```


Hämtar filtretypen.

**Returns:**
int – typen av filtret.
### getIndex() {#getIndex--}
```
public final int getIndex()
```


Hämtar indexet för ett [Filter](../../com.aspose.tasks/filter)-objekt i det objekt som innehåller Filters.

**Returns:**
int – indexet för ett [Filter](../../com.aspose.tasks/filter)-objekt i det objekt som innehåller Filters.
### getName() {#getName--}
```
public final String getName()
```


Hämtar namnet på ett Filter-objekt.

**Returns:**
java.lang.String – namnet på ett Filter-objekt.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Hämtar ett värde som anger om projektet visar filtreringsnamnet i Filter‑rullgardinslistan på fliken Visa i menyfliksområdet.

**Returns:**
boolean - ett värde som indikerar om projektet visar filternamnet i Filter‑rullgardinslistan på Visa‑fliken i Ribbon.
### getShowRelatedSummaryRows() {#getShowRelatedSummaryRows--}
```
public final boolean getShowRelatedSummaryRows()
```


Hämtar ett värde som anger om relaterade sammanfattningsrader visas för filtret.

**Returns:**
boolean - ett värde som indikerar om relaterade sammanfattningsrader visas för filtret.
### getUid() {#getUid--}
```
public final int getUid()
```


Hämtar den unika identifieraren för ett filter.

**Returns:**
int - den unika identifieraren för ett filter.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returnerar ett hash‑kodvärde för filtret.

**Returns:**
int - returnerar ett hash‑kodvärde för detta objekt.
### op_Equality(Filter a, Filter b) {#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Equality(Filter a, Filter b)
```


Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Det första filtret. |
| b | [Filter](../../com.aspose.tasks/filter) | Det andra filtret. |

**Returns:**
boolean - ett värde som indikerar om detta objekt är lika med ett specificerat objekt
### op_GreaterThan(Filter a, Filter b) {#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThan(Filter a, Filter b)
```


Returnerar ett värde som anger om detta objekt är större än ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Det första filtret. |
| b | [Filter](../../com.aspose.tasks/filter) | Det andra filtret. |

**Returns:**
boolean - ett värde som indikerar om detta objekt är större än ett specificerat objekt
### op_GreaterThanOrEqual(Filter a, Filter b) {#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThanOrEqual(Filter a, Filter b)
```


Returnerar ett värde som anger om detta objekt är större än eller lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Det första filtret. |
| b | [Filter](../../com.aspose.tasks/filter) | Det andra filtret. |

**Returns:**
boolean - ett värde som indikerar om detta objekt är större än eller lika med ett specificerat objekt
### op_Inequality(Filter a, Filter b) {#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Inequality(Filter a, Filter b)
```


Returnerar ett värde som anger om detta objekt inte är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Det första filtret. |
| b | [Filter](../../com.aspose.tasks/filter) | Det andra filtret. |

**Returns:**
boolean - ett värde som indikerar om detta objekt inte är lika med ett specificerat objekt
### op_LessThan(Filter a, Filter b) {#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThan(Filter a, Filter b)
```


Returnerar ett värde som anger om detta objekt är mindre än ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Det första filtret. |
| b | [Filter](../../com.aspose.tasks/filter) | Det andra filtret. |

**Returns:**
boolean - ett värde som indikerar om detta objekt är mindre än ett specificerat objekt
### op_LessThanOrEqual(Filter a, Filter b) {#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThanOrEqual(Filter a, Filter b)
```


Returnerar ett värde som anger om detta objekt är mindre än eller lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Det första filtret. |
| b | [Filter](../../com.aspose.tasks/filter) | Det andra filtret. |

**Returns:**
boolean - ett värde som indikerar om detta objekt är mindre än eller lika med ett specificerat objekt
### setCriteria(FilterCriteria value) {#setCriteria-com.aspose.tasks.FilterCriteria-}
```
public final void setCriteria(FilterCriteria value)
```


Ställer in kriterierna som uppgifter eller resurser måste uppfylla för att visas i MSP‑vyn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [FilterCriteria](../../com.aspose.tasks/filtercriteria) | kriterierna som uppgifter eller resurser måste uppfylla för att visas i MSP‑vyn. |

### setFilterType(int value) {#setFilterType-int-}
```
public final void setFilterType(int value)
```


Typen av filtret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | typen av filtret. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Ställer in namnet på ett Filter-objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | namnet på ett Filter‑objekt. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Ställer in ett värde som anger om projektet visar filtreringsnamnet i Filter‑rullgardinslistan på fliken Visa i menyfliksområdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om projektet visar filternamnet i Filter‑rullgardinslistan på Visa‑fliken i Ribbon. |

### setShowRelatedSummaryRows(boolean value) {#setShowRelatedSummaryRows-boolean-}
```
public final void setShowRelatedSummaryRows(boolean value)
```


Ställer in ett värde som anger om relaterade sammanfattningsrader visas för filtret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om relaterade sammanfattningsrader visas för filtret. |

