---
title: "PropertyKeyedCollection"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "فئة أساسية لمجموعة من الخصائص."
type: docs
weight: 231
url: /ar/java/com.aspose.tasks/propertykeyedcollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection

**All Implemented Interfaces:**
java.util.Collection
```
public abstract class PropertyKeyedCollection<T> extends PropertyCollection<T> implements Collection<T>
```

فئة أساسية لمجموعة من الخصائص.

T : نوع الخاصية.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [&lt;T1&gt;toArray(T1[] a)](#-T1-toArray-T1---) | \{@inheritDoc\} |
| [add(T item)](#add-T-) | ينشئ خاصية مخصصة جديدة. |
| [addAll(Collection&lt;? extends T&gt; c)](#addAll-java.util.Collection---extends-T--) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object item)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [contains(String name)](#contains-java.lang.String-) | يحدد ما إذا كان Aspose.Tasks.Properties.PropertyCollection<T> يحتوي على خاصية بالاسم المحدد. |
| [containsAll(Collection&lt;?&gt; c)](#containsAll-java.util.Collection----) | \{@inheritDoc\} |
| [getNames()](#getNames--) | يحصل على مجموعة جميع أسماء الخصائص. |
| [get_Item(String name)](#get-Item-java.lang.String-) | يحصل على الخاصية المرتبطة بالمفتاح المحدد. |
| [isEmpty()](#isEmpty--) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false. |
| [remove(Object item)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [removeAll(Collection&lt;?&gt; c)](#removeAll-java.util.Collection----) | \{@inheritDoc\} |
| [retainAll(Collection&lt;?&gt; c)](#retainAll-java.util.Collection----) | \{@inheritDoc\} |
| [size()](#size--) | يحصل على عدد الخصائص في المجموعة. |
| [toArray()](#toArray--) | \{@inheritDoc\} |
### &lt;T1&gt;toArray(T1[] a) {#-T1-toArray-T1---}
```
public T1[] <T1>toArray(T1[] a)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| أ | T1[] | \{@inheritDoc\} |

**Returns:**
T1[] - \{@inheritDoc\}
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


ينشئ خاصية مخصصة جديدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عنصر | T | الخاصية المراد إضافتها. |

**Returns:**
منطقي
### addAll(Collection&lt;? extends T&gt; c) {#addAll-java.util.Collection---extends-T--}
```
public boolean addAll(Collection<? extends T> c)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| c | java.util.Collection<? extends T> | \{@inheritDoc\} |

**Returns:**
منطقي - \{@inheritDoc\}
### clear() {#clear--}
```
public void clear()
```




### contains(Object item) {#contains-java.lang.Object-}
```
public final boolean contains(Object item)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عنصر | java.lang.Object |  |

**Returns:**
منطقي
### contains(String name) {#contains-java.lang.String-}
```
public final boolean contains(String name)
```


يحدد ما إذا كان Aspose.Tasks.Properties.PropertyCollection<T> يحتوي على خاصية بالاسم المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم خاصية |

**Returns:**
منطقي - true إذا كانت Aspose.Tasks.Properties.PropertyCollection<T> تحتوي على خاصية بالاسم المحدد؛ وإلا false.
### containsAll(Collection&lt;?&gt; c) {#containsAll-java.util.Collection----}
```
public boolean containsAll(Collection<?> c)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
منطقي - \{@inheritDoc\}
### getNames() {#getNames--}
```
public final Collection<String> getNames()
```


يحصل على مجموعة جميع أسماء الخصائص.

**Returns:**
java.util.Collection<java.lang.String> - مجموعة جميع أسماء الخصائص.
### get_Item(String name) {#get-Item-java.lang.String-}
```
public final T get_Item(String name)
```


يحصل على الخاصية المرتبطة بالمفتاح المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية المراد الحصول عليها. |

**Returns:**
T - الخاصية المرتبطة بالاسم المحدد.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```




**Returns:**
منطقي - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false.

**Returns:**
boolean - قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عنصر | java.lang.Object | \{@inheritDoc\} |

**Returns:**
منطقي - \{@inheritDoc\}
### removeAll(Collection&lt;?&gt; c) {#removeAll-java.util.Collection----}
```
public boolean removeAll(Collection<?> c)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
منطقي - \{@inheritDoc\}
### retainAll(Collection&lt;?&gt; c) {#retainAll-java.util.Collection----}
```
public boolean retainAll(Collection<?> c)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
منطقي - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


يحصل على عدد الخصائص في المجموعة.

**Returns:**
int - عدد الخصائص في المجموعة.
### toArray() {#toArray--}
```
public Object[] toArray()
```




**Returns:**
java.lang.Object[] - \{@inheritDoc\}
