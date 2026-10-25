---
title: "FilterCriteria"
second_title: "Aspose.Tasks for Java API Reference"
description: "Definisce i criteri che le attività o le risorse devono soddisfare per essere visualizzate nella vista MSP."
type: docs
weight: 94
url: /it/java/com.aspose.tasks/filtercriteria/
---

**Inheritance:**
java.lang.Object
```
public class FilterCriteria
```

Definisce i criteri che le attività o le risorse devono soddisfare per essere visualizzate nella vista MSP.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [FilterCriteria()](#FilterCriteria--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCriteriaRows()](#getCriteriaRows--) | Ottiene l'elenco delle righe figlio [FilterCriteria](../../com.aspose.tasks/filtercriteria). |
| [getField()](#getField--) | Ottiene un `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) da modificare. |
| [getOperation()](#getOperation--) | Ottiene il criterio stabilito con FieldName, Test e Value che si riferisce ad altri criteri nel filtro. |
| [getTest()](#getTest--) | Ottiene il tipo di confronto effettuato tra FieldName e Value che funge da criterio di selezione per il filtro. |
| [getValues()](#getValues--) | Ottiene i valori oggetto da confrontare con il valore del campo specificato con FieldName. |
| [isValueAField()](#isValueAField--) | Ottiene se il valore a destra di FilterCriteria è un riferimento a un campo, non un valore costante. |
| [isValueAField(int index)](#isValueAField-int-) | Ottiene se il valore all'indice di FilterCriteria è un riferimento a un campo, non un valore costante. |
| [setField(int value)](#setField-int-) | Imposta un `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) da modificare. |
| [setOperation(int value)](#setOperation-int-) | Imposta il criterio stabilito con FieldName, Test e Value che si riferisce ad altri criteri nel filtro. |
| [setTest(int value)](#setTest-int-) | Imposta il tipo di confronto effettuato tra FieldName e Value che funge da criterio di selezione per il filtro. |
| [setValue(int index, Object value)](#setValue-int-java.lang.Object-) | Imposta il valore oggetto all'indice da confrontare con il valore del campo specificato da FieldName. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Imposta il valore oggetto da confrontare con il valore del campo specificato da FieldName. |
| [setValueByField(int value)](#setValueByField-int-) | Imposta il campo il cui valore sarà confrontato con il valore del campo specificato da FieldName. |
| [setValueByField(int index, int value)](#setValueByField-int-int-) | Imposta il campo all'indice il cui valore sarà confrontato con il valore del campo specificato da FieldName. |
| [toString()](#toString--) | Restituisce la rappresentazione stringa dell'istanza della classe [FilterCriteria](../../com.aspose.tasks/filtercriteria). |
### FilterCriteria() {#FilterCriteria--}
```
public FilterCriteria()
```


### getCriteriaRows() {#getCriteriaRows--}
```
public final List<FilterCriteria> getCriteriaRows()
```


Ottiene l'elenco delle righe figlio [FilterCriteria](../../com.aspose.tasks/filtercriteria). Se il filtro contiene più di una riga di criterio, l'effetto dell'operatore And è che i criteri per entrambe le righe devono essere soddisfatti affinché l'attività o la risorsa venga visualizzata come risultato di questo filtro. L'effetto dell'operatore Or è che i criteri per una delle due righe devono essere soddisfatti.

**Returns:**
java.util.List&lt;com.aspose.tasks.FilterCriteria&gt; - l'elenco delle righe figlio [FilterCriteria](../../com.aspose.tasks/filtercriteria).
### getField() {#getField--}
```
public final int getField()
```


Ottiene un `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) da modificare.

**Returns:**
int - un `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) da modificare.
### getOperation() {#getOperation--}
```
public final int getOperation()
```


Ottiene il criterio stabilito con FieldName, Test e Value che si riferisce ad altri criteri nel filtro.

**Returns:**
int - il criterio stabilito con FieldName, Test e Value che si riferisce ad altri criteri nel filtro.
### getTest() {#getTest--}
```
public final int getTest()
```


Ottiene il tipo di confronto effettuato tra FieldName e Value che funge da criterio di selezione per il filtro. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - il tipo di confronto effettuato tra FieldName e Value che funge da criterio di selezione per il filtro.
### getValues() {#getValues--}
```
public final Object[] getValues()
```


Ottiene i valori oggetto da confrontare con il valore del campo specificato con FieldName.

**Returns:**
java.lang.Object[] - i valori oggetto da confrontare con il valore del campo specificato con FieldName.
### isValueAField() {#isValueAField--}
```
public final boolean isValueAField()
```


Ottiene se il valore a destra di FilterCriteria è un riferimento a un campo, non un valore costante.

**Returns:**
boolean - se il valore a destra di FilterCriteria è un riferimento a un campo, non un valore costante.
### isValueAField(int index) {#isValueAField-int-}
```
public final boolean isValueAField(int index)
```


Ottiene se il valore all'indice di FilterCriteria è un riferimento a un campo, non un valore costante.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | l'indice del valore |

**Returns:**
boolean - se il valore a destra dell'indice di FilterCriteria è un riferimento a un campo, non un valore costante.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Imposta un `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) da modificare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | int | un `Field`([getField()](../../com.aspose.tasks/filtercriteria\\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\\#setField-int-)) da modificare. |

### setOperation(int value) {#setOperation-int-}
```
public final void setOperation(int value)
```


Imposta il criterio stabilito con FieldName, Test e Value che si riferisce ad altri criteri nel filtro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il criterio stabilito con FieldName, Test e Value si riferisce ad altri criteri nel filtro. |

### setTest(int value) {#setTest-int-}
```
public final void setTest(int value)
```


Imposta il tipo di confronto effettuato tra FieldName e Value che funge da criterio di selezione per il filtro. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il tipo di confronto effettuato tra FieldName e Value che funge da criterio di selezione per il filtro. |

### setValue(int index, Object value) {#setValue-int-java.lang.Object-}
```
public final void setValue(int index, Object value)
```


Imposta il valore oggetto all'indice da confrontare con il valore del campo specificato da FieldName.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | l'indice del valore. |
| valore | java.lang.Object | valore oggetto che servirà come valore a destra dell'indice del criterio di filtro. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public final void setValue(Object value)
```


Imposta il valore oggetto da confrontare con il valore del campo specificato da FieldName.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object | valore oggetto che servirà come valore a destra del criterio di filtro. |

### setValueByField(int value) {#setValueByField-int-}
```
public final void setValueByField(int value)
```


Imposta il campo il cui valore sarà confrontato con il valore del campo specificato da FieldName.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | Campo che servirà come valore a destra del criterio di filtro. |

### setValueByField(int index, int value) {#setValueByField-int-int-}
```
public final void setValueByField(int index, int value)
```


Imposta il campo all'indice il cui valore sarà confrontato con il valore del campo specificato da FieldName.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | l'indice del valore |
| valore | int | Campo che servirà come valore a destra dell'indice del criterio di filtro. |

### toString() {#toString--}
```
public String toString()
```


Restituisce la rappresentazione stringa dell'istanza della classe [FilterCriteria](../../com.aspose.tasks/filtercriteria).

**Returns:**
java.lang.String - rappresentazione stringa di questo oggetto.
