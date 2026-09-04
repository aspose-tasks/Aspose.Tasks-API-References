---
title: "Filter"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt einen Filter im Projekt dar."
type: docs
weight: 91
url: /de/java/com.aspose.tasks/filter/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public final class Filter implements Comparable<Filter>, System.IEquatable<Filter>
```

Stellt einen Filter im Projekt dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Filter()](#Filter--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [compareTo(Filter other)](#compareTo-com.aspose.tasks.Filter-) | Vergleicht diese Instanz mit der angegebenen Instanz der [Filter](../../com.aspose.tasks/filter)-Klasse und gibt einen Hinweis auf ihre relative Reihenfolge zurück. |
| [equals(Filter other)](#equals-com.aspose.tasks.Filter-) | Gibt einen Wert zurück, der angibt, ob diese Instanz dem angegebenen AssignmentBaseline-Objekt gleich ist. |
| [equals(Object obj)](#equals-java.lang.Object-) | Gibt einen Wert zurück, der angibt, ob diese Instanz dem angegebenen AssignmentBaseline-Objekt gleich ist. |
| [getCriteria()](#getCriteria--) | Ermittelt die Kriterien, die Aufgaben oder Ressourcen erfüllen müssen, um in der MSP-Ansicht angezeigt zu werden. |
| [getFilterType()](#getFilterType--) | Ermittelt den Typ des Filters. |
| [getIndex()](#getIndex--) | Ermittelt den Index eines [Filter](../../com.aspose.tasks/filter)-Objekts im enthaltenden Filters-Objekt. |
| [getName()](#getName--) | Ermittelt den Namen eines Filter-Objekts. |
| [getShowInMenu()](#getShowInMenu--) | Ermittelt einen Wert, der angibt, ob das Projekt den Filternamen in der Filter‑Dropdown‑Liste auf der Registerkarte Ansicht im Menüband anzeigt. |
| [getShowRelatedSummaryRows()](#getShowRelatedSummaryRows--) | Ermittelt einen Wert, der angibt, ob zugehörige Summenzeilen für den Filter angezeigt werden. |
| [getUid()](#getUid--) | Ermittelt die eindeutige Kennung eines Filters. |
| [hashCode()](#hashCode--) | Gibt einen Hashcode-Wert für den Filter zurück. |
| [op_Equality(Filter a, Filter b)](#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [op_GreaterThan(Filter a, Filter b)](#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Gibt einen Wert zurück, der angibt, ob diese Instanz größer als ein angegebenes Objekt ist. |
| [op_GreaterThanOrEqual(Filter a, Filter b)](#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Gibt einen Wert zurück, der angibt, ob diese Instanz größer oder gleich einem angegebenen Objekt ist. |
| [op_Inequality(Filter a, Filter b)](#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Gibt einen Wert zurück, der angibt, ob diese Instanz nicht gleich einem angegebenen Objekt ist. |
| [op_LessThan(Filter a, Filter b)](#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Gibt einen Wert zurück, der angibt, ob diese Instanz kleiner als ein angegebenes Objekt ist. |
| [op_LessThanOrEqual(Filter a, Filter b)](#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Gibt einen Wert zurück, der angibt, ob diese Instanz kleiner oder gleich einem angegebenen Objekt ist. |
| [setCriteria(FilterCriteria value)](#setCriteria-com.aspose.tasks.FilterCriteria-) | Legt die Kriterien fest, die Aufgaben oder Ressourcen erfüllen müssen, um in der MSP-Ansicht angezeigt zu werden. |
| [setFilterType(int value)](#setFilterType-int-) | Der Typ des Filters. |
| [setName(String value)](#setName-java.lang.String-) | Legt den Namen eines Filter-Objekts fest. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Legt einen Wert fest, der angibt, ob das Projekt den Filternamen in der Filter‑Dropdown‑Liste auf der Registerkarte Ansicht im Menüband anzeigt. |
| [setShowRelatedSummaryRows(boolean value)](#setShowRelatedSummaryRows-boolean-) | Legt einen Wert fest, der angibt, ob zugehörige Summenzeilen für den Filter angezeigt werden. |
### Filter() {#Filter--}
```
public Filter()
```


### compareTo(Filter other) {#compareTo-com.aspose.tasks.Filter-}
```
public final int compareTo(Filter other)
```


Vergleicht diese Instanz mit der angegebenen Instanz der [Filter](../../com.aspose.tasks/filter)-Klasse und gibt einen Hinweis auf ihre relative Reihenfolge zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | die angegebene Instanz der [Filter](../../com.aspose.tasks/filter)-Klasse, die mit diesem Objekt verglichen wird. |

**Returns:**
int - ein Hinweis auf ihre relative Reihenfolge.
### equals(Filter other) {#equals-com.aspose.tasks.Filter-}
```
public final boolean equals(Filter other)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz dem angegebenen AssignmentBaseline-Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | das angegebene AssignmentBaseline-Objekt, das mit dieser Instanz verglichen wird. |

**Returns:**
boolean - gibt true zurück, wenn diese Instanz dem angegebenen AssignmentBaseline-Objekt gleich ist; andernfalls false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz dem angegebenen AssignmentBaseline-Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | das angegebene AssignmentBaseline-Objekt, das mit dieser Instanz verglichen wird. |

**Returns:**
boolean - gibt true zurück, wenn diese Instanz dem angegebenen AssignmentBaseline-Objekt gleich ist; andernfalls false.
### getCriteria() {#getCriteria--}
```
public final FilterCriteria getCriteria()
```


Ermittelt die Kriterien, die Aufgaben oder Ressourcen erfüllen müssen, um in der MSP-Ansicht angezeigt zu werden.

**Returns:**
[FilterCriteria](../../com.aspose.tasks/filtercriteria) - the criteria that tasks or resources must meet to be displayed in MSP view.
### getFilterType() {#getFilterType--}
```
public final int getFilterType()
```


Ermittelt den Typ des Filters.

**Returns:**
int - der Typ des Filters.
### getIndex() {#getIndex--}
```
public final int getIndex()
```


Ermittelt den Index eines [Filter](../../com.aspose.tasks/filter)-Objekts im enthaltenden Filters-Objekt.

**Returns:**
int - der Index eines [Filter](../../com.aspose.tasks/filter)-Objekts im enthaltenden Filters-Objekt.
### getName() {#getName--}
```
public final String getName()
```


Ermittelt den Namen eines Filter-Objekts.

**Returns:**
java.lang.String - der Name eines Filter-Objekts.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Ermittelt einen Wert, der angibt, ob das Projekt den Filternamen in der Filter‑Dropdown‑Liste auf der Registerkarte Ansicht im Menüband anzeigt.

**Returns:**
boolean - ein Wert, der angibt, ob das Projekt den Filternamen in der Dropdown-Liste Filter auf der Registerkarte Ansicht des Menübands anzeigt.
### getShowRelatedSummaryRows() {#getShowRelatedSummaryRows--}
```
public final boolean getShowRelatedSummaryRows()
```


Ermittelt einen Wert, der angibt, ob zugehörige Summenzeilen für den Filter angezeigt werden.

**Returns:**
boolean - ein Wert, der angibt, ob zugehörige Summenzeilen für den Filter angezeigt werden.
### getUid() {#getUid--}
```
public final int getUid()
```


Ermittelt die eindeutige Kennung eines Filters.

**Returns:**
int - die eindeutige Kennung eines Filters.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Gibt einen Hashcode-Wert für den Filter zurück.

**Returns:**
int - gibt einen Hashcode-Wert für dieses Objekt zurück.
### op_Equality(Filter a, Filter b) {#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Equality(Filter a, Filter b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Der erste Filter. |
| b | [Filter](../../com.aspose.tasks/filter) | Der zweite Filter. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist
### op_GreaterThan(Filter a, Filter b) {#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThan(Filter a, Filter b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz größer als ein angegebenes Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Der erste Filter. |
| b | [Filter](../../com.aspose.tasks/filter) | Der zweite Filter. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz größer als ein angegebenes Objekt ist
### op_GreaterThanOrEqual(Filter a, Filter b) {#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThanOrEqual(Filter a, Filter b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz größer oder gleich einem angegebenen Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Der erste Filter. |
| b | [Filter](../../com.aspose.tasks/filter) | Der zweite Filter. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz größer oder gleich einem angegebenen Objekt ist
### op_Inequality(Filter a, Filter b) {#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Inequality(Filter a, Filter b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz nicht gleich einem angegebenen Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Der erste Filter. |
| b | [Filter](../../com.aspose.tasks/filter) | Der zweite Filter. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz nicht gleich einem angegebenen Objekt ist
### op_LessThan(Filter a, Filter b) {#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThan(Filter a, Filter b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz kleiner als ein angegebenes Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Der erste Filter. |
| b | [Filter](../../com.aspose.tasks/filter) | Der zweite Filter. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz kleiner als ein angegebenes Objekt ist
### op_LessThanOrEqual(Filter a, Filter b) {#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThanOrEqual(Filter a, Filter b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz kleiner oder gleich einem angegebenen Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Der erste Filter. |
| b | [Filter](../../com.aspose.tasks/filter) | Der zweite Filter. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz kleiner oder gleich einem angegebenen Objekt ist
### setCriteria(FilterCriteria value) {#setCriteria-com.aspose.tasks.FilterCriteria-}
```
public final void setCriteria(FilterCriteria value)
```


Legt die Kriterien fest, die Aufgaben oder Ressourcen erfüllen müssen, um in der MSP-Ansicht angezeigt zu werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [FilterCriteria](../../com.aspose.tasks/filtercriteria) | die Kriterien, die Aufgaben oder Ressourcen erfüllen müssen, um in der MSP-Ansicht angezeigt zu werden. |

### setFilterType(int value) {#setFilterType-int-}
```
public final void setFilterType(int value)
```


Der Typ des Filters.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | der Typ des Filters. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Legt den Namen eines Filter-Objekts fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | der Name eines Filter-Objekts. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Legt einen Wert fest, der angibt, ob das Projekt den Filternamen in der Filter‑Dropdown‑Liste auf der Registerkarte Ansicht im Menüband anzeigt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob das Projekt den Filternamen in der Dropdown-Liste Filter auf der Registerkarte Ansicht des Menübands anzeigt. |

### setShowRelatedSummaryRows(boolean value) {#setShowRelatedSummaryRows-boolean-}
```
public final void setShowRelatedSummaryRows(boolean value)
```


Legt einen Wert fest, der angibt, ob zugehörige Summenzeilen für den Filter angezeigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob zugehörige Summenzeilen für den Filter angezeigt werden. |

