---
title: "RiskItemStatisticsCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Sammlung dar, die die Instanzen der  Klasse enthält."
type: docs
weight: 266
url: /de/java/com.aspose.tasks/riskitemstatisticscollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.util.Map, java.lang.Iterable
```
public class RiskItemStatisticsCollection implements Map<Task,RiskItemStatistics>, Iterable<RiskItemStatistics>
```

Stellt eine Sammlung dar, die die Instanzen der [RiskItemStatistics](../../com.aspose/tasks/riskitemstatistics) Klasse enthält.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [clear()](#clear--) | Entfernt alle Elemente aus der Sammlung. |
| [containsKey(Object key)](#containsKey-java.lang.Object-) | Gibt true zurück, wenn diese Map eine Zuordnung für den angegebenen Schlüssel enthält. |
| [containsValue(Object value)](#containsValue-java.lang.Object-) | Gibt true zurück, wenn diese Map einen oder mehrere Schlüssel auf den angegebenen Wert abbildet. |
| [entrySet()](#entrySet--) | Gibt eine Set-Ansicht der in dieser Map enthaltenen Zuordnungen zurück. |
| [get(Object task)](#get-java.lang.Object-) | Gibt eine Instanz der `RiskItemStatistics` Klasse zurück, die in dieser Sammlung enthalten ist und mit dem angegebenen Task-Objekt verknüpft ist; null, wenn das Element nicht gefunden wird. |
| [isEmpty()](#isEmpty--) | Gibt true zurück, wenn diese Map keine Schlüssel-Wert-Zuordnungen enthält |
| [iterator()](#iterator--) | Gibt einen Enumerator für diese Sammlung zurück. |
| [keySet()](#keySet--) | Gibt eine Set-Ansicht der in dieser Map enthaltenen Schlüssel zurück. |
| [put(Task key, RiskItemStatistics value)](#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-) | Verknüpft den angegebenen Wert mit dem angegebenen Schlüssel in dieser Map. |
| [putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m)](#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--) | Kopiert alle Zuordnungen von der angegebenen Map in diese Map. |
| [remove(Object key)](#remove-java.lang.Object-) | Entfernt die Zuordnung für einen Schlüssel aus dieser Map, falls sie vorhanden ist. |
| [size()](#size--) | Gibt die Anzahl der Elemente in dieser Sammlung zurück. |
| [values()](#values--) | Gibt eine Collection-Ansicht der in dieser Map enthaltenen Werte zurück. |
### clear() {#clear--}
```
public void clear()
```


Entfernt alle Elemente aus der Sammlung.

### containsKey(Object key) {#containsKey-java.lang.Object-}
```
public boolean containsKey(Object key)
```


Gibt true zurück, wenn diese Map eine Zuordnung für den angegebenen Schlüssel enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - true, wenn diese Map eine Zuordnung für den angegebenen Schlüssel enthält.
### containsValue(Object value) {#containsValue-java.lang.Object-}
```
public boolean containsValue(Object value)
```


Gibt true zurück, wenn diese Map einen oder mehrere Schlüssel auf den angegebenen Wert abbildet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - true, wenn diese Map einen oder mehrere Schlüssel auf den angegebenen Wert abbildet.
### entrySet() {#entrySet--}
```
public Set<Map.Entry<Task,RiskItemStatistics>> entrySet()
```


Gibt eine Set-Ansicht der in dieser Map enthaltenen Zuordnungen zurück.

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;com.aspose.tasks.Task,com.aspose.tasks.RiskItemStatistics&gt;&gt; - \{@inheritDoc\}
### get(Object task) {#get-java.lang.Object-}
```
public RiskItemStatistics get(Object task)
```


Gibt eine Instanz der `RiskItemStatistics` Klasse zurück, die in dieser Sammlung enthalten ist und mit dem angegebenen Task-Objekt verknüpft ist; null, wenn das Element nicht gefunden wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Aufgabe | java.lang.Object | die angegebene Instanz der `Task`-Klasse. |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - risk item which is associated with the specified task object if found; null otherwise.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Gibt true zurück, wenn diese Map keine Schlüssel-Wert-Zuordnungen enthält

**Returns:**
boolean - true, wenn diese Map keine Schlüssel-Wert-Zuordnungen enthält
### iterator() {#iterator--}
```
public Iterator<RiskItemStatistics> iterator()
```


Gibt einen Enumerator für diese Sammlung zurück.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.RiskItemStatistics&gt; - ein Enumerator für diese Sammlung.
### keySet() {#keySet--}
```
public Set<Task> keySet()
```


Gibt eine Set-Ansicht der in dieser Map enthaltenen Schlüssel zurück.

**Returns:**
java.util.Set&lt;com.aspose.tasks.Task&gt; - eine Mengenansicht der in dieser Map enthaltenen Schlüssel.
### put(Task key, RiskItemStatistics value) {#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-}
```
public RiskItemStatistics put(Task key, RiskItemStatistics value)
```


Verknüpft den angegebenen Wert mit dem angegebenen Schlüssel in dieser Map.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| key | [Task](../../com.aspose.tasks/task) | \{@inheritDoc\} |
| value | [RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m) {#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--}
```
public void putAll(Map<? extends Task,? extends RiskItemStatistics> m)
```


Kopiert alle Zuordnungen von der angegebenen Map in diese Map.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| m | java.util.Map&lt;? extends com.aspose.tasks.Task,? extends com.aspose.tasks.RiskItemStatistics&gt; | \{@inheritDoc\} |

### remove(Object key) {#remove-java.lang.Object-}
```
public RiskItemStatistics remove(Object key)
```


Entfernt die Zuordnung für einen Schlüssel aus dieser Map, falls sie vorhanden ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### size() {#size--}
```
public int size()
```


Gibt die Anzahl der Elemente in dieser Sammlung zurück.

**Returns:**
int - die Anzahl der Elemente in dieser Sammlung.
### values() {#values--}
```
public Collection<RiskItemStatistics> values()
```


Gibt eine Collection-Ansicht der in dieser Map enthaltenen Werte zurück.

**Returns:**
java.util.Collection&lt;com.aspose.tasks.RiskItemStatistics&gt; - eine Sammlungsansicht der in dieser Map enthaltenen Werte.
