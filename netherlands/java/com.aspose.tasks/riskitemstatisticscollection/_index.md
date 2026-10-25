---
title: "RiskItemStatisticsCollection"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een collectie voor die de instanties van de klasse bevat."
type: docs
weight: 266
url: /nl/java/com.aspose.tasks/riskitemstatisticscollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.util.Map, java.lang.Iterable
```
public class RiskItemStatisticsCollection implements Map<Task,RiskItemStatistics>, Iterable<RiskItemStatistics>
```

Stelt een collectie voor die de instanties van the [RiskItemStatistics](../../com.aspose/tasks/riskitemstatistics) klasse bevat.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [clear()](#clear--) | Verwijdert alle items uit de collectie. |
| [containsKey(Object key)](#containsKey-java.lang.Object-) | Retourneert true als deze map een mapping bevat voor de opgegeven sleutel. |
| [containsValue(Object value)](#containsValue-java.lang.Object-) | Retourneert true als deze map een of meer sleutels naar de opgegeven waarde mappt. |
| [entrySet()](#entrySet--) | Retourneert een Set-weergave van de mappings die in deze map zitten. |
| [get(Object task)](#get-java.lang.Object-) | Retourneert een instantie van de `RiskItemStatistics` klasse die zich in deze collectie bevindt en geassocieerd is met het opgegeven Task-object; null als het item niet wordt gevonden. |
| [isEmpty()](#isEmpty--) | Retourneert true als deze map geen sleutel-waarde mappings bevat |
| [iterator()](#iterator--) | Retourneert een enumerator voor deze collectie. |
| [keySet()](#keySet--) | Retourneert een Set-weergave van de sleutels die in deze map zitten. |
| [put(Task key, RiskItemStatistics value)](#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-) | Associeert de opgegeven waarde met de opgegeven sleutel in deze map. |
| [putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m)](#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--) | Kopieert alle mappings van de opgegeven map naar deze map. |
| [remove(Object key)](#remove-java.lang.Object-) | Verwijdert de mapping voor een sleutel uit deze map als deze aanwezig is. |
| [size()](#size--) | Retourneert het aantal elementen in deze collectie. |
| [values()](#values--) | Retourneert een Collection-weergave van de waarden die in deze map zitten. |
### clear() {#clear--}
```
public void clear()
```


Verwijdert alle items uit de collectie.

### containsKey(Object key) {#containsKey-java.lang.Object-}
```
public boolean containsKey(Object key)
```


Retourneert true als deze map een mapping bevat voor de opgegeven sleutel.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - true als deze map een mapping bevat voor de opgegeven sleutel.
### containsValue(Object value) {#containsValue-java.lang.Object-}
```
public boolean containsValue(Object value)
```


Retourneert true als deze map een of meer sleutels naar de opgegeven waarde mappt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - true als deze map een of meer sleutels naar de opgegeven waarde mappt.
### entrySet() {#entrySet--}
```
public Set<Map.Entry<Task,RiskItemStatistics>> entrySet()
```


Retourneert een Set-weergave van de mappings die in deze map zitten.

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;com.aspose.tasks.Task,com.aspose.tasks.RiskItemStatistics&gt;&gt; - \{@inheritDoc\}
### get(Object task) {#get-java.lang.Object-}
```
public RiskItemStatistics get(Object task)
```


Retourneert een instantie van de `RiskItemStatistics` klasse die zich in deze collectie bevindt en geassocieerd is met het opgegeven Task-object; null als het item niet wordt gevonden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| taak | java.lang.Object | de opgegeven instantie van de `Task` klasse. |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - risk item which is associated with the specified task object if found; null otherwise.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Retourneert true als deze map geen sleutel-waarde mappings bevat

**Returns:**
boolean - true als deze map geen sleutel-waarde koppelingen bevat
### iterator() {#iterator--}
```
public Iterator<RiskItemStatistics> iterator()
```


Retourneert een enumerator voor deze collectie.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.RiskItemStatistics&gt; - een enumerator voor deze collectie.
### keySet() {#keySet--}
```
public Set<Task> keySet()
```


Retourneert een Set-weergave van de sleutels die in deze map zitten.

**Returns:**
java.util.Set&lt;com.aspose.tasks.Task&gt; - een setweergave van de sleutels die in deze map zijn opgenomen.
### put(Task key, RiskItemStatistics value) {#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-}
```
public RiskItemStatistics put(Task key, RiskItemStatistics value)
```


Associeert de opgegeven waarde met de opgegeven sleutel in deze map.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| key | [Task](../../com.aspose.tasks/task) | \{@inheritDoc\} |
| value | [RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m) {#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--}
```
public void putAll(Map<? extends Task,? extends RiskItemStatistics> m)
```


Kopieert alle mappings van de opgegeven map naar deze map.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| m | java.util.Map&lt;? extends com.aspose.tasks.Task,? extends com.aspose.tasks.RiskItemStatistics&gt; | \{@inheritDoc\} |

### remove(Object key) {#remove-java.lang.Object-}
```
public RiskItemStatistics remove(Object key)
```


Verwijdert de mapping voor een sleutel uit deze map als deze aanwezig is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### size() {#size--}
```
public int size()
```


Retourneert het aantal elementen in deze collectie.

**Returns:**
int - het aantal elementen in deze collectie.
### values() {#values--}
```
public Collection<RiskItemStatistics> values()
```


Retourneert een Collection-weergave van de waarden die in deze map zitten.

**Returns:**
java.util.Collection&lt;com.aspose.tasks.RiskItemStatistics&gt; - een collectieweergave van de waarden die in deze map zijn opgenomen.
