---
title: "Filter"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een filter in Project voor."
type: docs
weight: 91
url: /nl/java/com.aspose.tasks/filter/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public final class Filter implements Comparable<Filter>, System.IEquatable<Filter>
```

Stelt een filter in Project voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Filter()](#Filter--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [compareTo(Filter other)](#compareTo-com.aspose.tasks.Filter-) | Vergelijkt deze instantie met de opgegeven instantie van de [Filter](../../com.aspose.tasks/filter) klasse en retourneert een indicatie van hun relatieve volgorde. |
| [equals(Filter other)](#equals-com.aspose.tasks.Filter-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven AssignmentBaseline-object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven AssignmentBaseline-object. |
| [getCriteria()](#getCriteria--) | Haalt de criteria op die taken of resources moeten voldoen om weergegeven te worden in de MSP-weergave. |
| [getFilterType()](#getFilterType--) | Haalt het type van de filter op. |
| [getIndex()](#getIndex--) | Haalt de index op van een [Filter](../../com.aspose.tasks/filter) object in het object dat de Filters bevat. |
| [getName()](#getName--) | Haalt de naam op van een Filter-object. |
| [getShowInMenu()](#getShowInMenu--) | Haalt een waarde op die aangeeft of het project de filternaam weergeeft in de vervolgkeuzelijst Filter op het tabblad Weergave van het lint. |
| [getShowRelatedSummaryRows()](#getShowRelatedSummaryRows--) | Haalt een waarde op die aangeeft of gerelateerde samenvattingsrijen worden weergegeven voor de filter. |
| [getUid()](#getUid--) | Haalt de unieke identifier op van een filter. |
| [hashCode()](#hashCode--) | Retourneert een hashcode-waarde voor de filter. |
| [op_Equality(Filter a, Filter b)](#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [op_GreaterThan(Filter a, Filter b)](#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Retourneert een waarde die aangeeft of deze instantie groter is dan een opgegeven object. |
| [op_GreaterThanOrEqual(Filter a, Filter b)](#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Retourneert een waarde die aangeeft of deze instantie groter dan of gelijk aan een opgegeven object is. |
| [op_Inequality(Filter a, Filter b)](#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Retourneert een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object. |
| [op_LessThan(Filter a, Filter b)](#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Retourneert een waarde die aangeeft of deze instantie kleiner is dan een opgegeven object. |
| [op_LessThanOrEqual(Filter a, Filter b)](#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Retourneert een waarde die aangeeft of deze instantie kleiner dan of gelijk aan een opgegeven object is. |
| [setCriteria(FilterCriteria value)](#setCriteria-com.aspose.tasks.FilterCriteria-) | Stelt de criteria in waaraan taken of resources moeten voldoen om weergegeven te worden in de MSP-weergave. |
| [setFilterType(int value)](#setFilterType-int-) | Het type van de filter. |
| [setName(String value)](#setName-java.lang.String-) | Stelt de naam in van een Filter-object. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Stelt een waarde in die aangeeft of het project de filternaam weergeeft in de vervolgkeuzelijst Filter op het tabblad Weergave van het lint. |
| [setShowRelatedSummaryRows(boolean value)](#setShowRelatedSummaryRows-boolean-) | Stelt een waarde in die aangeeft of gerelateerde samenvattingsrijen worden weergegeven voor de filter. |
### Filter() {#Filter--}
```
public Filter()
```


### compareTo(Filter other) {#compareTo-com.aspose.tasks.Filter-}
```
public final int compareTo(Filter other)
```


Vergelijkt deze instantie met de opgegeven instantie van de [Filter](../../com.aspose.tasks/filter) klasse en retourneert een indicatie van hun relatieve volgorde.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | de opgegeven instantie van de [Filter](../../com.aspose.tasks/filter) klasse om te vergelijken met dit object. |

**Returns:**
int - een indicatie van hun relatieve volgorde.
### equals(Filter other) {#equals-com.aspose.tasks.Filter-}
```
public final boolean equals(Filter other)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven AssignmentBaseline-object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | het opgegeven AssignmentBaseline-object om te vergelijken met deze instantie. |

**Returns:**
boolean - retourneert true als deze instantie gelijk is aan het opgegeven AssignmentBaseline-object; anders false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven AssignmentBaseline-object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | java.lang.Object | het opgegeven AssignmentBaseline-object om te vergelijken met deze instantie. |

**Returns:**
boolean - retourneert true als deze instantie gelijk is aan het opgegeven AssignmentBaseline-object; anders false.
### getCriteria() {#getCriteria--}
```
public final FilterCriteria getCriteria()
```


Haalt de criteria op die taken of resources moeten voldoen om weergegeven te worden in de MSP-weergave.

**Returns:**
[FilterCriteria](../../com.aspose.tasks/filtercriteria) - the criteria that tasks or resources must meet to be displayed in MSP view.
### getFilterType() {#getFilterType--}
```
public final int getFilterType()
```


Haalt het type van de filter op.

**Returns:**
int - het type van de filter.
### getIndex() {#getIndex--}
```
public final int getIndex()
```


Haalt de index op van een [Filter](../../com.aspose.tasks/filter) object in het object dat de Filters bevat.

**Returns:**
int - de index van een [Filter](../../com.aspose.tasks/filter) object in het object dat de Filters bevat.
### getName() {#getName--}
```
public final String getName()
```


Haalt de naam op van een Filter-object.

**Returns:**
java.lang.String - de naam van een Filter-object.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Haalt een waarde op die aangeeft of het project de filternaam weergeeft in de vervolgkeuzelijst Filter op het tabblad Weergave van het lint.

**Returns:**
boolean - een waarde die aangeeft of het project de filternaam toont in de vervolgkeuzelijst Filter op het tabblad Weergave van het lint.
### getShowRelatedSummaryRows() {#getShowRelatedSummaryRows--}
```
public final boolean getShowRelatedSummaryRows()
```


Haalt een waarde op die aangeeft of gerelateerde samenvattingsrijen worden weergegeven voor de filter.

**Returns:**
boolean - een waarde die aangeeft of gerelateerde samenvattingsrijen worden weergegeven voor het filter.
### getUid() {#getUid--}
```
public final int getUid()
```


Haalt de unieke identifier op van een filter.

**Returns:**
int - de unieke identifier van een filter.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Retourneert een hashcode-waarde voor de filter.

**Returns:**
int - retourneert een hashcode-waarde voor dit object.
### op_Equality(Filter a, Filter b) {#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Equality(Filter a, Filter b)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Het eerste filter. |
| b | [Filter](../../com.aspose.tasks/filter) | Het tweede filter. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object
### op_GreaterThan(Filter a, Filter b) {#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThan(Filter a, Filter b)
```


Retourneert een waarde die aangeeft of deze instantie groter is dan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Het eerste filter. |
| b | [Filter](../../com.aspose.tasks/filter) | Het tweede filter. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie groter is dan een opgegeven object
### op_GreaterThanOrEqual(Filter a, Filter b) {#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThanOrEqual(Filter a, Filter b)
```


Retourneert een waarde die aangeeft of deze instantie groter dan of gelijk aan een opgegeven object is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Het eerste filter. |
| b | [Filter](../../com.aspose.tasks/filter) | Het tweede filter. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie groter dan of gelijk aan een opgegeven object is
### op_Inequality(Filter a, Filter b) {#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Inequality(Filter a, Filter b)
```


Retourneert een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Het eerste filter. |
| b | [Filter](../../com.aspose.tasks/filter) | Het tweede filter. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object
### op_LessThan(Filter a, Filter b) {#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThan(Filter a, Filter b)
```


Retourneert een waarde die aangeeft of deze instantie kleiner is dan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Het eerste filter. |
| b | [Filter](../../com.aspose.tasks/filter) | Het tweede filter. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie kleiner is dan een opgegeven object
### op_LessThanOrEqual(Filter a, Filter b) {#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThanOrEqual(Filter a, Filter b)
```


Retourneert een waarde die aangeeft of deze instantie kleiner dan of gelijk aan een opgegeven object is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Het eerste filter. |
| b | [Filter](../../com.aspose.tasks/filter) | Het tweede filter. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie kleiner dan of gelijk aan een opgegeven object is
### setCriteria(FilterCriteria value) {#setCriteria-com.aspose.tasks.FilterCriteria-}
```
public final void setCriteria(FilterCriteria value)
```


Stelt de criteria in waaraan taken of resources moeten voldoen om weergegeven te worden in de MSP-weergave.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [FilterCriteria](../../com.aspose.tasks/filtercriteria) | de criteria waaraan taken of resources moeten voldoen om weergegeven te worden in de MSP-weergave. |

### setFilterType(int value) {#setFilterType-int-}
```
public final void setFilterType(int value)
```


Het type van de filter.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het type van het filter. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Stelt de naam in van een Filter-object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de naam van een Filter-object. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Stelt een waarde in die aangeeft of het project de filternaam weergeeft in de vervolgkeuzelijst Filter op het tabblad Weergave van het lint.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of het project de filternaam toont in de vervolgkeuzelijst Filter op het tabblad Weergave van het lint. |

### setShowRelatedSummaryRows(boolean value) {#setShowRelatedSummaryRows-boolean-}
```
public final void setShowRelatedSummaryRows(boolean value)
```


Stelt een waarde in die aangeeft of gerelateerde samenvattingsrijen worden weergegeven voor de filter.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of gerelateerde samenvattingsrijen worden weergegeven voor het filter. |

