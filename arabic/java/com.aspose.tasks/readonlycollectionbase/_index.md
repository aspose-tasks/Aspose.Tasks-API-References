---
title: "ReadOnlyCollectionBase"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل مجموعة للقراءة فقط من الكائنات."
type: docs
weight: 238
url: /ar/java/com.aspose.tasks/readonlycollectionbase/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class ReadOnlyCollectionBase<T> extends AbstractList<T>
```

يمثل مجموعة للقراءة فقط من الكائنات.

T : نوع عناصر المجموعة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(T item)](#add-T-) | هذه هي تنفيذية النموذج لطريقة Add في ICollection، التي تُطلق فقط UnsupportedOperationException |
| [add(int index, T element)](#add-int-T-) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | يعيد العنصر في الفهرس المحدد. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | يحدد ما إذا كانت المجموعة للقراءة فقط. |
| [iterator()](#iterator--) | يرجع مُعدِّدًا لهذه المجموعة. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [set(int index, T value)](#set-int-T-) | يعيد العنصر في الفهرس المحدد. |
| [size()](#size--) | يحصل على عدد الكائنات المحتواة في الكائن. |
| [toList()](#toList--) | يحول المجموعة إلى قائمة من الكائنات. |
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


هذه هي تنفيذية النموذج لطريقة Add في ICollection، التي تُطلق فقط UnsupportedOperationException

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عنصر | T | العنصر المراد إضافته. |

**Returns:**
منطقي
### add(int index, T element) {#add-int-T-}
```
public final void add(int index, T element)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | \{@inheritDoc\} |
| العنصر | T | \{@inheritDoc\} |

### clear() {#clear--}
```
public final void clear()
```




### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
منطقي - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public final T get(int index)
```


يعيد العنصر في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الفهرس الصفري للعنصر المراد الحصول عليه. |

**Returns:**
T - العنصر في الفهرس المحدد.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


يحدد ما إذا كانت المجموعة للقراءة فقط.

**Returns:**
boolean - صحيح إذا كانت المجموعة للقراءة فقط؛ خطأ غير ذلك.
### iterator() {#iterator--}
```
public final Iterator<T> iterator()
```


يرجع مُعدِّدًا لهذه المجموعة.

**Returns:**
java.util.Iterator&lt;T&gt; - عداد لهذه المجموعة.
### remove(int index) {#remove-int-}
```
public final T remove(int index)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | \{@inheritDoc\} |

**Returns:**
T - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
منطقي - \{@inheritDoc\}
### set(int index, T value) {#set-int-T-}
```
public final T set(int index, T value)
```


يعيد العنصر في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | الفهرس الصفري للعنصر المراد الحصول عليه. |
| القيمة | T |  |

**Returns:**
T - العنصر في الفهرس المحدد.
### size() {#size--}
```
public final int size()
```


يحصل على عدد الكائنات المحتواة في الكائن.

**Returns:**
int - عدد الكائنات المحتواة في الكائن.
### toList() {#toList--}
```
public final List<T> toList()
```


يحول المجموعة إلى قائمة من الكائنات.

**Returns:**
java.util.List&lt;T&gt; - قائمة عامة من الكائنات.
