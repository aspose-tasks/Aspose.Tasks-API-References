---
title: "FilterCollection"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يحتوي على قائمة من الكائنات."
type: docs
weight: 92
url: /ar/java/com.aspose.tasks/filtercollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class FilterCollection extends AbstractCollection<Filter>
```

يحتوي على قائمة من كائنات [Filter](../../com.aspose.tasks/filter). ينفّذ واجهة ICollection&lt;Filter&gt;.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(Filter item)](#add-com.aspose.tasks.Filter-) |  |
| [clear()](#clear--) | يزيل جميع العناصر من هذه المجموعة (عملية اختيارية). |
| [contains(Filter item)](#contains-com.aspose.tasks.Filter-) | يرجع true إذا كانت هذه المجموعة تحتوي على العنصر المحدد. |
| [copyTo(Filter[] array, int arrayIndex)](#copyTo-com.aspose.tasks.Filter---int-) | ينسخ العناصر من المصفوفة المحددة إلى هذه المجموعة بدءًا من الفهرس المحدد. |
| [iterator()](#iterator--) | يرجع مكرّرًا للعناصر الموجودة في هذه المجموعة. |
| [remove(Filter item)](#remove-com.aspose.tasks.Filter-) | يزيل العنصر المحدد من هذه المجموعة. |
| [size()](#size--) | يحصل على عدد العناصر الموجودة في هذه المجموعة. |
| [toList()](#toList--) | يحوِّل مجموعة الفلاتر إلى قائمة من كائنات `Filter`. |
### add(Filter item) {#add-com.aspose.tasks.Filter-}
```
public boolean add(Filter item)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) |  |

**Returns:**
منطقي
### clear() {#clear--}
```
public void clear()
```


يزيل جميع العناصر من هذه المجموعة (عملية اختيارية).

### contains(Filter item) {#contains-com.aspose.tasks.Filter-}
```
public final boolean contains(Filter item)
```


يرجع true إذا كانت هذه المجموعة تحتوي على العنصر المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | العنصر المحدد. |

**Returns:**
boolean - true إذا كانت المجموعة تحتوي على العنصر المحدد.
### copyTo(Filter[] array, int arrayIndex) {#copyTo-com.aspose.tasks.Filter---int-}
```
public final void copyTo(Filter[] array, int arrayIndex)
```


ينسخ العناصر من المصفوفة المحددة إلى هذه المجموعة بدءًا من الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| array | [Filter\[\]](../../com.aspose.tasks/filter) | المصفوفة الأحادية الأبعاد المحددة لنسخ العناصر إليها |
| arrayIndex | int | الفهرس الصفري للمصفوفة المحددة الذي يبدأ عنده النسخ. |

### iterator() {#iterator--}
```
public Iterator<Filter> iterator()
```


يرجع مكرّرًا للعناصر الموجودة في هذه المجموعة.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Filter&gt; - مكرِّر المجموعة.
### remove(Filter item) {#remove-com.aspose.tasks.Filter-}
```
public final boolean remove(Filter item)
```


يزيل العنصر المحدد من هذه المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | العنصر المحدد. |

**Returns:**
boolean - true إذا كانت العملية ناجحة.
### size() {#size--}
```
public final int size()
```


يحصل على عدد العناصر الموجودة في هذه المجموعة.

**Returns:**
int - عدد العناصر الموجودة في هذه المجموعة.
### toList() {#toList--}
```
public List<Filter> toList()
```


يحوِّل مجموعة الفلاتر إلى قائمة من كائنات `Filter`.

**Returns:**
java.util.List&lt;com.aspose.tasks.Filter&gt; - قائمة عامة من كائنات `Filter`.
