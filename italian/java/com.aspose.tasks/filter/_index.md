---
title: "Filter"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un filtro in Project."
type: docs
weight: 91
url: /it/java/com.aspose.tasks/filter/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public final class Filter implements Comparable<Filter>, System.IEquatable<Filter>
```

Rappresenta un filtro in Project.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Filter()](#Filter--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [compareTo(Filter other)](#compareTo-com.aspose.tasks.Filter-) | Confronta questa istanza con l'istanza specificata della classe [Filter](../../com.aspose.tasks/filter) e restituisce un'indicazione del loro ordine relativo. |
| [equals(Filter other)](#equals-com.aspose.tasks.Filter-) | Restituisce un valore che indica se questa istanza è uguale all'oggetto AssignmentBaseline specificato. |
| [equals(Object obj)](#equals-java.lang.Object-) | Restituisce un valore che indica se questa istanza è uguale all'oggetto AssignmentBaseline specificato. |
| [getCriteria()](#getCriteria--) | Ottiene i criteri che attività o risorse devono soddisfare per essere visualizzati nella vista MSP. |
| [getFilterType()](#getFilterType--) | Ottiene il tipo del filtro. |
| [getIndex()](#getIndex--) | Restituisce l'indice di un oggetto [Filter](../../com.aspose.tasks/filter) nell'oggetto contenitore Filters. |
| [getName()](#getName--) | Restituisce il nome di un oggetto Filter. |
| [getShowInMenu()](#getShowInMenu--) | Restituisce un valore che indica se il progetto mostra il nome del filtro nell'elenco a discesa Filter nella scheda Visualizza del Ribbon. |
| [getShowRelatedSummaryRows()](#getShowRelatedSummaryRows--) | Restituisce un valore che indica se le righe di riepilogo correlate sono visualizzate per il filtro. |
| [getUid()](#getUid--) | Restituisce l'identificatore univoco di un filtro. |
| [hashCode()](#hashCode--) | Restituisce un valore di codice hash per il filtro. |
| [op_Equality(Filter a, Filter b)](#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [op_GreaterThan(Filter a, Filter b)](#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Restituisce un valore che indica se questa istanza è maggiore di un oggetto specificato. |
| [op_GreaterThanOrEqual(Filter a, Filter b)](#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Restituisce un valore che indica se questa istanza è maggiore o uguale a un oggetto specificato. |
| [op_Inequality(Filter a, Filter b)](#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Restituisce un valore che indica se questa istanza non è uguale a un oggetto specificato. |
| [op_LessThan(Filter a, Filter b)](#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Restituisce un valore che indica se questa istanza è minore di un oggetto specificato. |
| [op_LessThanOrEqual(Filter a, Filter b)](#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Restituisce un valore che indica se questa istanza è minore o uguale a un oggetto specificato. |
| [setCriteria(FilterCriteria value)](#setCriteria-com.aspose.tasks.FilterCriteria-) | Imposta i criteri che le attività o le risorse devono soddisfare per essere visualizzate nella vista MSP. |
| [setFilterType(int value)](#setFilterType-int-) | Il tipo del filtro. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome di un oggetto Filter. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Imposta un valore che indica se il progetto mostra il nome del filtro nell'elenco a discesa Filter nella scheda Visualizza del Ribbon. |
| [setShowRelatedSummaryRows(boolean value)](#setShowRelatedSummaryRows-boolean-) | Imposta un valore che indica se le righe di riepilogo correlate sono visualizzate per il filtro. |
### Filter() {#Filter--}
```
public Filter()
```


### compareTo(Filter other) {#compareTo-com.aspose.tasks.Filter-}
```
public final int compareTo(Filter other)
```


Confronta questa istanza con l'istanza specificata della classe [Filter](../../com.aspose.tasks/filter) e restituisce un'indicazione del loro ordine relativo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | l'istanza specificata della classe [Filter](../../com.aspose.tasks/filter) da confrontare con questo oggetto. |

**Returns:**
int - un'indicazione del loro ordine relativo.
### equals(Filter other) {#equals-com.aspose.tasks.Filter-}
```
public final boolean equals(Filter other)
```


Restituisce un valore che indica se questa istanza è uguale all'oggetto AssignmentBaseline specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | l'oggetto AssignmentBaseline specificato da confrontare con questa istanza. |

**Returns:**
boolean - restituisce true se questa istanza è uguale all'oggetto AssignmentBaseline specificato; altrimenti, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Restituisce un valore che indica se questa istanza è uguale all'oggetto AssignmentBaseline specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | l'oggetto AssignmentBaseline specificato da confrontare con questa istanza. |

**Returns:**
boolean - restituisce true se questa istanza è uguale all'oggetto AssignmentBaseline specificato; altrimenti, false.
### getCriteria() {#getCriteria--}
```
public final FilterCriteria getCriteria()
```


Ottiene i criteri che attività o risorse devono soddisfare per essere visualizzati nella vista MSP.

**Returns:**
[FilterCriteria](../../com.aspose.tasks/filtercriteria) - the criteria that tasks or resources must meet to be displayed in MSP view.
### getFilterType() {#getFilterType--}
```
public final int getFilterType()
```


Ottiene il tipo del filtro.

**Returns:**
int - il tipo del filtro.
### getIndex() {#getIndex--}
```
public final int getIndex()
```


Restituisce l'indice di un oggetto [Filter](../../com.aspose.tasks/filter) nell'oggetto contenitore Filters.

**Returns:**
int - l'indice di un oggetto [Filter](../../com.aspose.tasks/filter) nell'oggetto contenitore Filters.
### getName() {#getName--}
```
public final String getName()
```


Restituisce il nome di un oggetto Filter.

**Returns:**
java.lang.String - il nome di un oggetto Filter.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Restituisce un valore che indica se il progetto mostra il nome del filtro nell'elenco a discesa Filter nella scheda Visualizza del Ribbon.

**Returns:**
boolean - un valore che indica se il progetto mostra il nome del filtro nell'elenco a discesa Filtri nella scheda Visualizza del nastro.
### getShowRelatedSummaryRows() {#getShowRelatedSummaryRows--}
```
public final boolean getShowRelatedSummaryRows()
```


Restituisce un valore che indica se le righe di riepilogo correlate sono visualizzate per il filtro.

**Returns:**
boolean - un valore che indica se le righe di riepilogo correlate vengono visualizzate per il filtro.
### getUid() {#getUid--}
```
public final int getUid()
```


Restituisce l'identificatore univoco di un filtro.

**Returns:**
int - l'identificatore univoco di un filtro.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Restituisce un valore di codice hash per il filtro.

**Returns:**
int - restituisce un valore di codice hash per questo oggetto.
### op_Equality(Filter a, Filter b) {#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Equality(Filter a, Filter b)
```


Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Il primo filtro. |
| b | [Filter](../../com.aspose.tasks/filter) | Il secondo filtro. |

**Returns:**
boolean - un valore che indica se questa istanza è uguale a un oggetto specificato
### op_GreaterThan(Filter a, Filter b) {#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThan(Filter a, Filter b)
```


Restituisce un valore che indica se questa istanza è maggiore di un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Il primo filtro. |
| b | [Filter](../../com.aspose.tasks/filter) | Il secondo filtro. |

**Returns:**
boolean - un valore che indica se questa istanza è maggiore di un oggetto specificato
### op_GreaterThanOrEqual(Filter a, Filter b) {#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThanOrEqual(Filter a, Filter b)
```


Restituisce un valore che indica se questa istanza è maggiore o uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Il primo filtro. |
| b | [Filter](../../com.aspose.tasks/filter) | Il secondo filtro. |

**Returns:**
boolean - un valore che indica se questa istanza è maggiore o uguale a un oggetto specificato
### op_Inequality(Filter a, Filter b) {#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Inequality(Filter a, Filter b)
```


Restituisce un valore che indica se questa istanza non è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Il primo filtro. |
| b | [Filter](../../com.aspose.tasks/filter) | Il secondo filtro. |

**Returns:**
boolean - un valore che indica se questa istanza non è uguale a un oggetto specificato
### op_LessThan(Filter a, Filter b) {#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThan(Filter a, Filter b)
```


Restituisce un valore che indica se questa istanza è minore di un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Il primo filtro. |
| b | [Filter](../../com.aspose.tasks/filter) | Il secondo filtro. |

**Returns:**
boolean - un valore che indica se questa istanza è minore di un oggetto specificato
### op_LessThanOrEqual(Filter a, Filter b) {#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThanOrEqual(Filter a, Filter b)
```


Restituisce un valore che indica se questa istanza è minore o uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Il primo filtro. |
| b | [Filter](../../com.aspose.tasks/filter) | Il secondo filtro. |

**Returns:**
boolean - un valore che indica se questa istanza è minore o uguale a un oggetto specificato
### setCriteria(FilterCriteria value) {#setCriteria-com.aspose.tasks.FilterCriteria-}
```
public final void setCriteria(FilterCriteria value)
```


Imposta i criteri che le attività o le risorse devono soddisfare per essere visualizzate nella vista MSP.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [FilterCriteria](../../com.aspose.tasks/filtercriteria) | i criteri che attività o risorse devono soddisfare per essere visualizzati nella vista MSP. |

### setFilterType(int value) {#setFilterType-int-}
```
public final void setFilterType(int value)
```


Il tipo del filtro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il tipo del filtro. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Imposta il nome di un oggetto Filter.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il nome di un oggetto Filter. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Imposta un valore che indica se il progetto mostra il nome del filtro nell'elenco a discesa Filter nella scheda Visualizza del Ribbon.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se il progetto mostra il nome del filtro nell'elenco a discesa Filtri nella scheda Visualizza del nastro. |

### setShowRelatedSummaryRows(boolean value) {#setShowRelatedSummaryRows-boolean-}
```
public final void setShowRelatedSummaryRows(boolean value)
```


Imposta un valore che indica se le righe di riepilogo correlate sono visualizzate per il filtro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se le righe di riepilogo correlate vengono visualizzate per il filtro. |

