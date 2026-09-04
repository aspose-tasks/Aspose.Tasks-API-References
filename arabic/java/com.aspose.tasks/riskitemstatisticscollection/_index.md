---
title: "RiskItemStatisticsCollection"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل مجموعة تحتوي على مثيلات الفئة."
type: docs
weight: 266
url: /ar/java/com.aspose.tasks/riskitemstatisticscollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.util.Map, java.lang.Iterable
```
public class RiskItemStatisticsCollection implements Map<Task,RiskItemStatistics>, Iterable<RiskItemStatistics>
```

يمثل مجموعة تحتوي على مثيلات الفئة [RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [clear()](#clear--) | يزيل جميع العناصر من المجموعة. |
| [containsKey(Object key)](#containsKey-java.lang.Object-) | يرجع true إذا كان هذا الخريطة يحتوي على تعيين للمفتاح المحدد. |
| [containsValue(Object value)](#containsValue-java.lang.Object-) | يرجع true إذا كان هذا الخريطة يربط مفتاحًا أو أكثر بالقيمة المحددة. |
| [entrySet()](#entrySet--) | يرجع عرض Set للتعيينات المحتواة في هذا الخريطة. |
| [get(Object task)](#get-java.lang.Object-) | يرجع مثيلًا من الفئة `RiskItemStatistics` الموجود في هذه المجموعة والمتعلق بكائن Task المحدد؛ null إذا لم يتم العثور على العنصر. |
| [isEmpty()](#isEmpty--) | يرجع true إذا كان هذا الخريطة لا يحتوي على أي تعيينات مفتاح-قيمة |
| [iterator()](#iterator--) | يرجع مُعدِّدًا لهذه المجموعة. |
| [keySet()](#keySet--) | يرجع عرض Set للمفاتيح الموجودة في هذا الخريطة. |
| [put(Task key, RiskItemStatistics value)](#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-) | يربط القيمة المحددة بالمفتاح المحدد في هذا الخريطة. |
| [putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m)](#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--) | ينسخ جميع التعيينات من الخريطة المحددة إلى هذا الخريطة. |
| [remove(Object key)](#remove-java.lang.Object-) | يزيل التعيين للمفتاح من هذا الخريطة إذا كان موجودًا. |
| [size()](#size--) | يعيد عدد العناصر في هذه المجموعة. |
| [values()](#values--) | يرجع عرض Collection للقيم الموجودة في هذا الخريطة. |
### clear() {#clear--}
```
public void clear()
```


يزيل جميع العناصر من المجموعة.

### containsKey(Object key) {#containsKey-java.lang.Object-}
```
public boolean containsKey(Object key)
```


يرجع true إذا كان هذا الخريطة يحتوي على تعيين للمفتاح المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - true إذا كان هذا الخريطة يحتوي على تعيين للمفتاح المحدد.
### containsValue(Object value) {#containsValue-java.lang.Object-}
```
public boolean containsValue(Object value)
```


يرجع true إذا كان هذا الخريطة يربط مفتاحًا أو أكثر بالقيمة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - true إذا كان هذا الخريطة يربط مفتاحًا أو أكثر بالقيمة المحددة.
### entrySet() {#entrySet--}
```
public Set<Map.Entry<Task,RiskItemStatistics>> entrySet()
```


يرجع عرض Set للتعيينات المحتواة في هذا الخريطة.

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;com.aspose.tasks.Task,com.aspose.tasks.RiskItemStatistics&gt;&gt; - \{@inheritDoc\}
### get(Object task) {#get-java.lang.Object-}
```
public RiskItemStatistics get(Object task)
```


يرجع مثيلًا من الفئة `RiskItemStatistics` الموجود في هذه المجموعة والمتعلق بكائن Task المحدد؛ null إذا لم يتم العثور على العنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| مهمة | java.lang.Object | المثيل المحدد من الفئة `Task`. |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - risk item which is associated with the specified task object if found; null otherwise.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


يرجع true إذا كان هذا الخريطة لا يحتوي على أي تعيينات مفتاح-قيمة

**Returns:**
boolean - صحيح إذا كانت هذه الخريطة لا تحتوي على أي تعيينات مفتاح-قيمة
### iterator() {#iterator--}
```
public Iterator<RiskItemStatistics> iterator()
```


يرجع مُعدِّدًا لهذه المجموعة.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.RiskItemStatistics&gt; - عداد لهذه المجموعة.
### keySet() {#keySet--}
```
public Set<Task> keySet()
```


يرجع عرض Set للمفاتيح الموجودة في هذا الخريطة.

**Returns:**
java.util.Set&lt;com.aspose.tasks.Task&gt; - عرض مجموعة للمفاتيح الموجودة في هذه الخريطة.
### put(Task key, RiskItemStatistics value) {#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-}
```
public RiskItemStatistics put(Task key, RiskItemStatistics value)
```


يربط القيمة المحددة بالمفتاح المحدد في هذا الخريطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| key | [Task](../../com.aspose.tasks/task) | \{@inheritDoc\} |
| value | [RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m) {#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--}
```
public void putAll(Map<? extends Task,? extends RiskItemStatistics> m)
```


ينسخ جميع التعيينات من الخريطة المحددة إلى هذا الخريطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| m | java.util.Map&lt;? extends com.aspose.tasks.Task,? extends com.aspose.tasks.RiskItemStatistics&gt; | \{@inheritDoc\} |

### remove(Object key) {#remove-java.lang.Object-}
```
public RiskItemStatistics remove(Object key)
```


يزيل التعيين للمفتاح من هذا الخريطة إذا كان موجودًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### size() {#size--}
```
public int size()
```


يعيد عدد العناصر في هذه المجموعة.

**Returns:**
int - عدد العناصر في هذه المجموعة.
### values() {#values--}
```
public Collection<RiskItemStatistics> values()
```


يرجع عرض Collection للقيم الموجودة في هذا الخريطة.

**Returns:**
java.util.Collection&lt;com.aspose.tasks.RiskItemStatistics&gt; - عرض مجموعة للقيم الموجودة في هذه الخريطة.
