---
title: "TimephasedDataCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una raccolta di oggetti."
type: docs
weight: 321
url: /it/java/com.aspose.tasks/timephaseddatacollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class TimephasedDataCollection extends AbstractList<TimephasedData>
```

Rappresenta una raccolta di oggetti [TimephasedData](../../com.aspose.tasks/timephaseddata).
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TimephasedDataCollection()](#TimephasedDataCollection--) | Inizializza una nuova istanza della classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(TimephasedData item)](#add-com.aspose.tasks.TimephasedData-) | Aggiunge un'istanza di [TimephasedData](../../com.aspose.tasks/timephaseddata) a questo oggetto di raccolta. |
| [addRange(Iterable&lt;TimephasedData&gt; timephasedCollection)](#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--) | Aggiunge una raccolta di istanze di [TimephasedData](../../com.aspose.tasks/timephaseddata) a questo oggetto di raccolta. |
| [clear()](#clear--) | Rimuove tutti gli elementi dalla [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). |
| [containsItem(TimephasedData item)](#containsItem-com.aspose.tasks.TimephasedData-) | Determina se la [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contiene un valore specifico. |
| [copyToTArray(TimephasedData[] array, int arrayIndex)](#copyToTArray-com.aspose.tasks.TimephasedData---int-) | Copia gli elementi della [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) in un Array, iniziando da un indice specifico dell'Array. |
| [get(int index)](#get-int-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Ottiene un valore che indica se System.Collections.Generic.ICollection&lt;T&gt; è di sola lettura. |
| [iterator()](#iterator--) | Restituisce un iteratore per questa raccolta. |
| [remove(TimephasedData item)](#remove-com.aspose.tasks.TimephasedData-) | Rimuove l'istanza di [TimephasedData](../../com.aspose.tasks/timephaseddata) da questo oggetto di raccolta. |
| [selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)](#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-) | Seleziona tutte le fasi temporali tra `startTime` e `finishTime`. |
| [set_Item(int index, TimephasedData value)](#set-Item-int-com.aspose.tasks.TimephasedData-) | Imposta l'elemento all'indice specificato. |
| [size()](#size--) | Ottiene il numero di oggetti contenuti in questo oggetto [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). |
| [toList()](#toList--) | Converte l'oggetto [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) in un elenco di oggetti [TimephasedData](../../com.aspose.tasks/timephaseddata). |
### TimephasedDataCollection() {#TimephasedDataCollection--}
```
public TimephasedDataCollection()
```


Inizializza una nuova istanza della classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).

### add(TimephasedData item) {#add-com.aspose.tasks.TimephasedData-}
```
public final boolean add(TimephasedData item)
```


Aggiunge un'istanza di [TimephasedData](../../com.aspose.tasks/timephaseddata) a questo oggetto di raccolta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | L'elemento da aggiungere. |

**Returns:**
boolean - true, se l'elemento è stato aggiunto; altrimenti false.
### addRange(Iterable&lt;TimephasedData&gt; timephasedCollection) {#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--}
```
public final void addRange(Iterable<TimephasedData> timephasedCollection)
```


Aggiunge una raccolta di istanze di [TimephasedData](../../com.aspose.tasks/timephaseddata) a questo oggetto di raccolta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| timephasedCollection | java.lang.Iterable&lt;com.aspose.tasks.TimephasedData&gt; | Una raccolta di oggetti [TimephasedData](../../com.aspose.tasks/timephaseddata) da aggiungere. |

### clear() {#clear--}
```
public final void clear()
```


Rimuove tutti gli elementi dalla [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).

### containsItem(TimephasedData item) {#containsItem-com.aspose.tasks.TimephasedData-}
```
public final boolean containsItem(TimephasedData item)
```


Determina se la [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contiene un valore specifico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | L'oggetto da individuare nella raccolta. |

**Returns:**
boolean - true se `item` è trovato nella raccolta; altrimenti false.
### copyToTArray(TimephasedData[] array, int arrayIndex) {#copyToTArray-com.aspose.tasks.TimephasedData---int-}
```
public final void copyToTArray(TimephasedData[] array, int arrayIndex)
```


Copia gli elementi della [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) in un Array, iniziando da un indice specifico dell'Array.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| array | [TimephasedData\[\]](../../com.aspose.tasks/timephaseddata) | L'Array monodimensionale che è la destinazione degli elementi copiati da [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). L'Array deve avere un indice basato su zero. |
| arrayIndex | int | L'indice basato su zero in `array` a partire dal quale inizia la copia. |

### get(int index) {#get-int-}
```
public TimephasedData get(int index)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Ottiene un valore che indica se System.Collections.Generic.ICollection&lt;T&gt; è di sola lettura.

**Returns:**
boolean - true se la System.Collections.Generic.ICollection<T> è di sola lettura; altrimenti, false.
### iterator() {#iterator--}
```
public final Iterator<TimephasedData> iterator()
```


Restituisce un iteratore per questa raccolta.

**Returns:**
java.util.Iterator<com.aspose.tasks.TimephasedData> - un iteratore per questa raccolta.
### remove(TimephasedData item) {#remove-com.aspose.tasks.TimephasedData-}
```
public final boolean remove(TimephasedData item)
```


Rimuove l'istanza di [TimephasedData](../../com.aspose.tasks/timephaseddata) da questo oggetto di raccolta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | L'elemento da rimuovere. |

**Returns:**
boolean - true se `item` è stato rimosso correttamente dalla [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection); altrimenti, false. Questo metodo restituisce false anche se `item` non è stato trovato nella [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).
### selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime) {#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-}
```
public final List<TimephasedData> selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)
```


Seleziona tutte le fasi temporali tra `startTime` e `finishTime`. Ha una complessità O(log n) nel caso medio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| timephasedDataType | byte | Tipo di fasi temporali da selezionare. |
| startTime | java.util.Date | Inizio dell'intervallo. |
| finishTime | java.util.Date | Fine dell'intervallo. |

**Returns:**
java.util.List<com.aspose.tasks.TimephasedData> - Restituisce una nuova istanza di lista dei dati [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) ordinati per la proprietà Start.
### set_Item(int index, TimephasedData value) {#set-Item-int-com.aspose.tasks.TimephasedData-}
```
public final void set_Item(int index, TimephasedData value)
```


Imposta l'elemento all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | L'indice basato su zero dell'elemento da impostare. |
| value | [TimephasedData](../../com.aspose.tasks/timephaseddata) | l'elemento da impostare. |

### size() {#size--}
```
public final int size()
```


Ottiene il numero di oggetti contenuti in questo oggetto [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).

**Returns:**
int - il numero di oggetti contenuti in questo oggetto [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).
### toList() {#toList--}
```
public final List<TimephasedData> toList()
```


Converte l'oggetto [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) in un elenco di oggetti [TimephasedData](../../com.aspose.tasks/timephaseddata).

**Returns:**
java.util.List<com.aspose.tasks.TimephasedData> - Elenco di oggetti [TimephasedData](../../com.aspose.tasks/timephaseddata).
