---
title: "RiskItemStatisticsCollection"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Belirtilen sınıfın örneklerini içeren bir koleksiyonu temsil eder."
type: docs
weight: 266
url: /tr/java/com.aspose.tasks/riskitemstatisticscollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.util.Map, java.lang.Iterable
```
public class RiskItemStatisticsCollection implements Map<Task,RiskItemStatistics>, Iterable<RiskItemStatistics>
```

[RiskItemStatistics](../../com.aspose/tasks/riskitemstatistics) sınıfının örneklerini içeren bir koleksiyonu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [clear()](#clear--) | Koleksiyondaki tüm öğeleri kaldırır. |
| [containsKey(Object key)](#containsKey-java.lang.Object-) | Belirtilen anahtar için bir eşleme içeriyorsa true döndürür. |
| [containsValue(Object value)](#containsValue-java.lang.Object-) | Belirtilen değer için bir veya daha fazla anahtarı eşliyorsa true döndürür. |
| [entrySet()](#entrySet--) | Bu haritada bulunan eşlemelerin bir Set görünümünü döndürür. |
| [get(Object task)](#get-java.lang.Object-) | Belirtilen Task nesnesiyle ilişkili bu koleksiyonda bulunan `RiskItemStatistics` sınıfının bir örneğini döndürür; öğe bulunamazsa null. |
| [isEmpty()](#isEmpty--) | Bu harita hiçbir anahtar-değer eşlemesi içermiyorsa true döndürür. |
| [iterator()](#iterator--) | Bu koleksiyon için bir enumerator döndürür. |
| [keySet()](#keySet--) | Bu haritada bulunan anahtarların bir Set görünümünü döndürür. |
| [put(Task key, RiskItemStatistics value)](#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-) | Belirtilen değeri bu haritada belirtilen anahtarla ilişkilendirir. |
| [putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m)](#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--) | Belirtilen haritadan tüm eşlemeleri bu haritaya kopyalar. |
| [remove(Object key)](#remove-java.lang.Object-) | Bir anahtar için eşlemeyi, mevcutsa bu haritadan kaldırır. |
| [size()](#size--) | Bu koleksiyondaki öğe sayısını döndürür. |
| [values()](#values--) | Bu haritada bulunan değerlerin bir Collection görünümünü döndürür. |
### clear() {#clear--}
```
public void clear()
```


Koleksiyondaki tüm öğeleri kaldırır.

### containsKey(Object key) {#containsKey-java.lang.Object-}
```
public boolean containsKey(Object key)
```


Belirtilen anahtar için bir eşleme içeriyorsa true döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - belirtilen anahtar için bir eşleme içeriyorsa true.
### containsValue(Object value) {#containsValue-java.lang.Object-}
```
public boolean containsValue(Object value)
```


Belirtilen değer için bir veya daha fazla anahtarı eşliyorsa true döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - belirtilen değer için bir veya daha fazla anahtarı eşliyorsa true.
### entrySet() {#entrySet--}
```
public Set<Map.Entry<Task,RiskItemStatistics>> entrySet()
```


Bu haritada bulunan eşlemelerin bir Set görünümünü döndürür.

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;com.aspose.tasks.Task,com.aspose.tasks.RiskItemStatistics&gt;&gt; - \{@inheritDoc\}
### get(Object task) {#get-java.lang.Object-}
```
public RiskItemStatistics get(Object task)
```


Belirtilen Task nesnesiyle ilişkili bu koleksiyonda bulunan `RiskItemStatistics` sınıfının bir örneğini döndürür; öğe bulunamazsa null.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| görev | java.lang.Object | Belirtilen `Task` sınıfının örneği. |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - risk item which is associated with the specified task object if found; null otherwise.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Bu harita hiçbir anahtar-değer eşlemesi içermiyorsa true döndürür.

**Returns:**
boolean - bu harita hiçbir anahtar-değer eşlemesi içermiyorsa true
### iterator() {#iterator--}
```
public Iterator<RiskItemStatistics> iterator()
```


Bu koleksiyon için bir enumerator döndürür.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.RiskItemStatistics&gt; - bu koleksiyon için bir yineleyici.
### keySet() {#keySet--}
```
public Set<Task> keySet()
```


Bu haritada bulunan anahtarların bir Set görünümünü döndürür.

**Returns:**
java.util.Set&lt;com.aspose.tasks.Task&gt; - bu haritada bulunan anahtarların bir küme görünümü.
### put(Task key, RiskItemStatistics value) {#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-}
```
public RiskItemStatistics put(Task key, RiskItemStatistics value)
```


Belirtilen değeri bu haritada belirtilen anahtarla ilişkilendirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| key | [Task](../../com.aspose.tasks/task) | \{@inheritDoc\} |
| value | [RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m) {#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--}
```
public void putAll(Map<? extends Task,? extends RiskItemStatistics> m)
```


Belirtilen haritadan tüm eşlemeleri bu haritaya kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| m | java.util.Map&lt;? extends com.aspose.tasks.Task,? extends com.aspose.tasks.RiskItemStatistics&gt; | \{@inheritDoc\} |

### remove(Object key) {#remove-java.lang.Object-}
```
public RiskItemStatistics remove(Object key)
```


Bir anahtar için eşlemeyi, mevcutsa bu haritadan kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### size() {#size--}
```
public int size()
```


Bu koleksiyondaki öğe sayısını döndürür.

**Returns:**
int - bu koleksiyondaki öğe sayısı.
### values() {#values--}
```
public Collection<RiskItemStatistics> values()
```


Bu haritada bulunan değerlerin bir Collection görünümünü döndürür.

**Returns:**
java.util.Collection&lt;com.aspose.tasks.RiskItemStatistics&gt; - bu haritada bulunan değerlerin bir koleksiyon görünümü.
