---
title: "RiskItemStatisticsCollection"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en samling som innehåller instanser av klassen."
type: docs
weight: 266
url: /sv/java/com.aspose.tasks/riskitemstatisticscollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.util.Map, java.lang.Iterable
```
public class RiskItemStatisticsCollection implements Map<Task,RiskItemStatistics>, Iterable<RiskItemStatistics>
```

Representerar en samling som innehåller instanser av klassen [RiskItemStatistics](../../com.aspose/tasks/riskitemstatistics).
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [clear()](#clear--) | Tar bort alla objekt från samlingen. |
| [containsKey(Object key)](#containsKey-java.lang.Object-) | Returnerar true om denna map innehåller en mappning för den angivna nyckeln. |
| [containsValue(Object value)](#containsValue-java.lang.Object-) | Returnerar true om denna map mappar en eller flera nycklar till det angivna värdet. |
| [entrySet()](#entrySet--) | Returnerar en Set-vy av mappningarna som finns i denna map. |
| [get(Object task)](#get-java.lang.Object-) | Returnerar en instans av klassen `RiskItemStatistics` som finns i denna samling och som är associerad med det angivna Task-objektet; null om objektet inte hittas. |
| [isEmpty()](#isEmpty--) | Returnerar true om denna map inte innehåller några nyckel‑värde‑mappningar |
| [iterator()](#iterator--) | Returnerar en enumerator för denna samling. |
| [keySet()](#keySet--) | Returnerar en Set-vy av nycklarna som finns i denna map. |
| [put(Task key, RiskItemStatistics value)](#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-) | Associerar det angivna värdet med den angivna nyckeln i denna map. |
| [putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m)](#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--) | Kopierar alla mappningar från den angivna map till denna map. |
| [remove(Object key)](#remove-java.lang.Object-) | Tar bort mappningen för en nyckel från denna map om den finns. |
| [size()](#size--) | Returnerar antalet element i denna samling. |
| [values()](#values--) | Returnerar en Collection-vy av värdena som finns i denna map. |
### clear() {#clear--}
```
public void clear()
```


Tar bort alla objekt från samlingen.

### containsKey(Object key) {#containsKey-java.lang.Object-}
```
public boolean containsKey(Object key)
```


Returnerar true om denna map innehåller en mappning för den angivna nyckeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - true om denna map innehåller en mappning för den angivna nyckeln.
### containsValue(Object value) {#containsValue-java.lang.Object-}
```
public boolean containsValue(Object value)
```


Returnerar true om denna map mappar en eller flera nycklar till det angivna värdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - true om denna map mappar en eller flera nycklar till det angivna värdet.
### entrySet() {#entrySet--}
```
public Set<Map.Entry<Task,RiskItemStatistics>> entrySet()
```


Returnerar en Set-vy av mappningarna som finns i denna map.

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;com.aspose.tasks.Task,com.aspose.tasks.RiskItemStatistics&gt;&gt; - \\{@inheritDoc\\}
### get(Object task) {#get-java.lang.Object-}
```
public RiskItemStatistics get(Object task)
```


Returnerar en instans av klassen `RiskItemStatistics` som finns i denna samling och som är associerad med det angivna Task-objektet; null om objektet inte hittas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uppgift | java.lang.Object | den angivna instansen av klassen `Task`. |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - risk item which is associated with the specified task object if found; null otherwise.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Returnerar true om denna map inte innehåller några nyckel‑värde‑mappningar

**Returns:**
boolean - sant om denna karta inte innehåller några nyckel‑värde‑par
### iterator() {#iterator--}
```
public Iterator<RiskItemStatistics> iterator()
```


Returnerar en enumerator för denna samling.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.RiskItemStatistics&gt; - en enumerator för denna samling.
### keySet() {#keySet--}
```
public Set<Task> keySet()
```


Returnerar en Set-vy av nycklarna som finns i denna map.

**Returns:**
java.util.Set&lt;com.aspose.tasks.Task&gt; - en mängdvy av nycklarna som finns i denna karta.
### put(Task key, RiskItemStatistics value) {#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-}
```
public RiskItemStatistics put(Task key, RiskItemStatistics value)
```


Associerar det angivna värdet med den angivna nyckeln i denna map.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| key | [Task](../../com.aspose.tasks/task) | \{@inheritDoc\} |
| value | [RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m) {#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--}
```
public void putAll(Map<? extends Task,? extends RiskItemStatistics> m)
```


Kopierar alla mappningar från den angivna map till denna map.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| m | java.util.Map&lt;? extends com.aspose.tasks.Task,? extends com.aspose.tasks.RiskItemStatistics&gt; | \{@inheritDoc\} |

### remove(Object key) {#remove-java.lang.Object-}
```
public RiskItemStatistics remove(Object key)
```


Tar bort mappningen för en nyckel från denna map om den finns.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### size() {#size--}
```
public int size()
```


Returnerar antalet element i denna samling.

**Returns:**
int - antalet element i denna samling.
### values() {#values--}
```
public Collection<RiskItemStatistics> values()
```


Returnerar en Collection-vy av värdena som finns i denna map.

**Returns:**
java.util.Collection&lt;com.aspose.tasks.RiskItemStatistics&gt; - en samlingsvy av värdena som finns i denna karta.
