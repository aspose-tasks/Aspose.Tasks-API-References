---
title: "RateCollection"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل مجموعة تحتوي على كائنات."
type: docs
weight: 234
url: /ar/java/com.aspose.tasks/ratecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractMap

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RateCollection extends AbstractMap<Integer,RateByDateCollection> implements Iterable<Map.Entry<Integer,RateByDateCollection>>
```

يمثل مجموعة تحتوي على كائنات [Rate](../../com.aspose.tasks/rate).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(Date ratesFrom)](#add-java.util.Date-) | يضيف نسخة جديدة من [Rate](../../com.aspose.tasks/rate) إلى هذه المجموعة. |
| [add(Date ratesFrom, int type)](#add-java.util.Date-int-) | يضيف نسخة جديدة من [Rate](../../com.aspose.tasks/rate) إلى هذه المجموعة. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [entrySet()](#entrySet--) | (@inheritDoc\\} |
| [get(Object key)](#get-java.lang.Object-) | (@inheritDoc\\} |
| [getByRateType(int key)](#getByRateType-int-) | يعيد العنصر في الفهرس المحدد. |
| [getParentResource()](#getParentResource--) | يحصل على كائن [Resource](../../com.aspose.tasks/resource) الأب لهذه المجموعة. |
| [isReadOnly()](#isReadOnly--) | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط. |
| [iterator()](#iterator--) | يرجع مُعدِّدًا لهذه المجموعة. |
| [put(Integer key, RateByDateCollection value)](#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-) | (@inheritDoc\\} |
| [remove(Rate item)](#remove-com.aspose.tasks.Rate-) | يزيل نسخة Rate من هذه المجموعة. |
| [setByRateType(int key, RateByDateCollection value)](#setByRateType-int-com.aspose.tasks.RateByDateCollection-) | يضبط العنصر في الفهرس المحدد. |
| [size()](#size--) | يحصل على عدد العناصر الموجودة في RateCollection. |
| [toList()](#toList--) | يحول كائن [RateCollection](../../com.aspose.tasks/ratecollection) إلى قائمة من كائنات [Rate](../../com.aspose.tasks/rate). |
| [toList(int type)](#toList-int-) | يحول كائن [RateCollection](../../com.aspose.tasks/ratecollection) إلى قائمة من كائنات [Rate](../../com.aspose.tasks/rate) مُفلترة حسب نوع [RateType](../../com.aspose.tasks/ratetype) المحدد. |
### add(Date ratesFrom) {#add-java.util.Date-}
```
public final Rate add(Date ratesFrom)
```


يضيف نسخة جديدة من [Rate](../../com.aspose.tasks/rate) إلى هذه المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ratesFrom | java.util.Date | التاريخ الذي يبدأ فيه سريان السعر الجديد. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### add(Date ratesFrom, int type) {#add-java.util.Date-int-}
```
public final Rate add(Date ratesFrom, int type)
```


يضيف نسخة جديدة من [Rate](../../com.aspose.tasks/rate) إلى هذه المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ratesFrom | java.util.Date | التاريخ الذي يبدأ فيه سريان السعر الجديد. |
| type | int | جدول الأسعار لإضافته. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### clear() {#clear--}
```
public final void clear()
```




### entrySet() {#entrySet--}
```
public Set<Map.Entry<Integer,RateByDateCollection>> entrySet()
```


(@inheritDoc\\}

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;java.lang.Integer,com.aspose.tasks.RateByDateCollection&gt;&gt; - \{@inheritDoc\}
### get(Object key) {#get-java.lang.Object-}
```
public final RateByDateCollection get(Object key)
```


(@inheritDoc\\}

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### getByRateType(int key) {#getByRateType-int-}
```
public final RateByDateCollection getByRateType(int key)
```


يعيد العنصر في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| key | int | الفهرس الصفري للعنصر المراد الحصول عليه. |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - the element at the specified index.
### getParentResource() {#getParentResource--}
```
public final Resource getParentResource()
```


يحصل على كائن [Resource](../../com.aspose.tasks/resource) الأب لهذه المجموعة.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the parent [Resource](../../com.aspose.tasks/resource) object for this collection.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط.

**Returns:**
boolean - قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط.
### iterator() {#iterator--}
```
public final Iterator iterator()
```


يرجع مُعدِّدًا لهذه المجموعة.

**Returns:**
java.util.Iterator - عداد لهذه المجموعة.
### put(Integer key, RateByDateCollection value) {#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-}
```
public final RateByDateCollection put(Integer key, RateByDateCollection value)
```


(@inheritDoc\\}

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| key | java.lang.Integer | \{@inheritDoc\} |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### remove(Rate item) {#remove-com.aspose.tasks.Rate-}
```
public final boolean remove(Rate item)
```


يزيل نسخة Rate من هذه المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| item | [Rate](../../com.aspose.tasks/rate) | العنصر المراد إزالته. |

**Returns:**
منطقي - true إذا تمت إزالة Rate المحدد بنجاح؛ وإلا false.
### setByRateType(int key, RateByDateCollection value) {#setByRateType-int-com.aspose.tasks.RateByDateCollection-}
```
public final void setByRateType(int key, RateByDateCollection value)
```


يضبط العنصر في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| key | int | الفهرس الصفري للعنصر الذي سيتم تعيينه. |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | العنصر الذي سيتم تعيينه في الفهرس المحدد. |

### size() {#size--}
```
public final int size()
```


يحصل على عدد العناصر الموجودة في RateCollection.

**Returns:**
int - عدد العناصر الموجودة في RateCollection.
### toList() {#toList--}
```
public final List<Rate> toList()
```


يحول كائن [RateCollection](../../com.aspose.tasks/ratecollection) إلى قائمة من كائنات [Rate](../../com.aspose.tasks/rate).

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - قائمة من كائنات [Rate](../../com.aspose.tasks/rate).
### toList(int type) {#toList-int-}
```
public final List<Rate> toList(int type)
```


يحول كائن [RateCollection](../../com.aspose.tasks/ratecollection) إلى قائمة من كائنات [Rate](../../com.aspose.tasks/rate) مُفلترة حسب نوع [RateType](../../com.aspose.tasks/ratetype) المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | النوع المراد تصفيته. |

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - قائمة من كائنات [Rate](../../com.aspose.tasks/rate).
