---
title: "RiskItemStatisticsCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una raccolta contenente le istanze della classe."
type: docs
weight: 266
url: /it/java/com.aspose.tasks/riskitemstatisticscollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.util.Map, java.lang.Iterable
```
public class RiskItemStatisticsCollection implements Map<Task,RiskItemStatistics>, Iterable<RiskItemStatistics>
```

Rappresenta una collezione contenente le istanze della classe [RiskItemStatistics](../../com.aspose/tasks/riskitemstatistics).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [clear()](#clear--) | Rimuove tutti gli elementi dalla collezione. |
| [containsKey(Object key)](#containsKey-java.lang.Object-) | Restituisce true se questa mappa contiene una corrispondenza per la chiave specificata. |
| [containsValue(Object value)](#containsValue-java.lang.Object-) | Restituisce true se questa mappa associa una o più chiavi al valore specificato. |
| [entrySet()](#entrySet--) | Restituisce una visualizzazione Set delle associazioni contenute in questa mappa. |
| [get(Object task)](#get-java.lang.Object-) | Restituisce un'istanza della classe `RiskItemStatistics` contenuta in questa collezione che è associata all'oggetto Task specificato; null se l'elemento non viene trovato. |
| [isEmpty()](#isEmpty--) | Restituisce true se questa mappa non contiene associazioni chiave-valore |
| [iterator()](#iterator--) | Restituisce un enumeratore per questa collezione. |
| [keySet()](#keySet--) | Restituisce una visualizzazione Set delle chiavi contenute in questa mappa. |
| [put(Task key, RiskItemStatistics value)](#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-) | Associa il valore specificato alla chiave specificata in questa mappa. |
| [putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m)](#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--) | Copia tutte le associazioni dalla mappa specificata a questa mappa. |
| [remove(Object key)](#remove-java.lang.Object-) | Rimuove l'associazione per una chiave da questa mappa se è presente. |
| [size()](#size--) | Restituisce il numero di elementi in questa raccolta. |
| [values()](#values--) | Restituisce una visualizzazione Collection dei valori contenuti in questa mappa. |
### clear() {#clear--}
```
public void clear()
```


Rimuove tutti gli elementi dalla collezione.

### containsKey(Object key) {#containsKey-java.lang.Object-}
```
public boolean containsKey(Object key)
```


Restituisce true se questa mappa contiene una corrispondenza per la chiave specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - true se questa mappa contiene una corrispondenza per la chiave specificata.
### containsValue(Object value) {#containsValue-java.lang.Object-}
```
public boolean containsValue(Object value)
```


Restituisce true se questa mappa associa una o più chiavi al valore specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - true se questa mappa associa una o più chiavi al valore specificato.
### entrySet() {#entrySet--}
```
public Set<Map.Entry<Task,RiskItemStatistics>> entrySet()
```


Restituisce una visualizzazione Set delle associazioni contenute in questa mappa.

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;com.aspose.tasks.Task,com.aspose.tasks.RiskItemStatistics&gt;&gt; - \{@inheritDoc\}
### get(Object task) {#get-java.lang.Object-}
```
public RiskItemStatistics get(Object task)
```


Restituisce un'istanza della classe `RiskItemStatistics` contenuta in questa collezione che è associata all'oggetto Task specificato; null se l'elemento non viene trovato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| attività | java.lang.Object | l'istanza specificata della classe `Task`. |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - risk item which is associated with the specified task object if found; null otherwise.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Restituisce true se questa mappa non contiene associazioni chiave-valore

**Returns:**
boolean - vero se questa mappa non contiene associazioni chiave-valore
### iterator() {#iterator--}
```
public Iterator<RiskItemStatistics> iterator()
```


Restituisce un enumeratore per questa collezione.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.RiskItemStatistics&gt; - un enumeratore per questa collezione.
### keySet() {#keySet--}
```
public Set<Task> keySet()
```


Restituisce una visualizzazione Set delle chiavi contenute in questa mappa.

**Returns:**
java.util.Set&lt;com.aspose.tasks.Task&gt; - una vista a set delle chiavi contenute in questa mappa.
### put(Task key, RiskItemStatistics value) {#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-}
```
public RiskItemStatistics put(Task key, RiskItemStatistics value)
```


Associa il valore specificato alla chiave specificata in questa mappa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| key | [Task](../../com.aspose.tasks/task) | \{@inheritDoc\} |
| value | [RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m) {#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--}
```
public void putAll(Map<? extends Task,? extends RiskItemStatistics> m)
```


Copia tutte le associazioni dalla mappa specificata a questa mappa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| m | java.util.Map&lt;? extends com.aspose.tasks.Task,? extends com.aspose.tasks.RiskItemStatistics&gt; | \{@inheritDoc\} |

### remove(Object key) {#remove-java.lang.Object-}
```
public RiskItemStatistics remove(Object key)
```


Rimuove l'associazione per una chiave da questa mappa se è presente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### size() {#size--}
```
public int size()
```


Restituisce il numero di elementi in questa raccolta.

**Returns:**
int - il numero di elementi in questa collezione.
### values() {#values--}
```
public Collection<RiskItemStatistics> values()
```


Restituisce una visualizzazione Collection dei valori contenuti in questa mappa.

**Returns:**
java.util.Collection&lt;com.aspose.tasks.RiskItemStatistics&gt; - una vista di collezione dei valori contenuti in questa mappa.
