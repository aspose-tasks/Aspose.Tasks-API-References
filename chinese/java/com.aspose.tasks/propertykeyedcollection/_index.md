---
title: "PropertyKeyedCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "属性集合的基类。"
type: docs
weight: 231
url: /zh/java/com.aspose.tasks/propertykeyedcollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection

**All Implemented Interfaces:**
java.util.Collection
```
public abstract class PropertyKeyedCollection<T> extends PropertyCollection<T> implements Collection<T>
```

属性集合的基类。

T : 属性的类型。
## 方法

| 方法 | 描述 |
| --- | --- |
| [&lt;T1&gt;toArray(T1[] a)](#-T1-toArray-T1---) | \{@inheritDoc\} |
| [add(T item)](#add-T-) | 创建一个新的自定义属性。 |
| [addAll(Collection&lt;? extends T&gt; c)](#addAll-java.util.Collection---extends-T--) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object item)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [contains(String name)](#contains-java.lang.String-) | 确定 Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; 是否包含具有指定名称的属性。 |
| [containsAll(Collection&lt;?&gt; c)](#containsAll-java.util.Collection----) | \{@inheritDoc\} |
| [getNames()](#getNames--) | 获取所有属性名称的集合。 |
| [get_Item(String name)](#get-Item-java.lang.String-) | 获取与指定键关联的属性。 |
| [isEmpty()](#isEmpty--) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | 获取一个值，指示此集合是否为只读；否则为 false。 |
| [remove(Object item)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [removeAll(Collection&lt;?&gt; c)](#removeAll-java.util.Collection----) | \{@inheritDoc\} |
| [retainAll(Collection&lt;?&gt; c)](#retainAll-java.util.Collection----) | \{@inheritDoc\} |
| [size()](#size--) | 获取集合中属性的数量。 |
| [toArray()](#toArray--) | \{@inheritDoc\} |
### &lt;T1&gt;toArray(T1[] a) {#-T1-toArray-T1---}
```
public T1[] <T1>toArray(T1[] a)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 一个 | T1[] | \{@inheritDoc\} |

**Returns:**
T1[] - \\{@inheritDoc\\}
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


创建一个新的自定义属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 项 | T | 要添加的属性。 |

**Returns:**
boolean
### addAll(Collection&lt;? extends T&gt; c) {#addAll-java.util.Collection---extends-T--}
```
public boolean addAll(Collection<? extends T> c)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| c | java.util.Collection&lt;? extends T&gt; | \{@inheritDoc\} |

**Returns:**
布尔 - \{@inheritDoc\}
### clear() {#clear--}
```
public void clear()
```




### contains(Object item) {#contains-java.lang.Object-}
```
public final boolean contains(Object item)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 项 | java.lang.Object |  |

**Returns:**
boolean
### contains(String name) {#contains-java.lang.String-}
```
public final boolean contains(String name)
```


确定 Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; 是否包含具有指定名称的属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String | 属性的名称 |

**Returns:**
boolean - 如果 Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; 包含具有指定名称的属性，则为 true；否则为 false。
### containsAll(Collection&lt;?&gt; c) {#containsAll-java.util.Collection----}
```
public boolean containsAll(Collection<?> c)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \{@inheritDoc\} |

**Returns:**
布尔 - \{@inheritDoc\}
### getNames() {#getNames--}
```
public final Collection<String> getNames()
```


获取所有属性名称的集合。

**Returns:**
java.util.Collection&lt;java.lang.String&gt; - 所有属性名称的集合。
### get_Item(String name) {#get-Item-java.lang.String-}
```
public final T get_Item(String name)
```


获取与指定键关联的属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String | 要获取的属性的名称。 |

**Returns:**
T - 与指定名称关联的属性。
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```




**Returns:**
布尔 - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


获取一个值，指示此集合是否为只读；否则为 false。

**Returns:**
boolean - 一个值，指示此集合是否为只读；否则为 false。
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 项 | java.lang.Object | \{@inheritDoc\} |

**Returns:**
布尔 - \{@inheritDoc\}
### removeAll(Collection&lt;?&gt; c) {#removeAll-java.util.Collection----}
```
public boolean removeAll(Collection<?> c)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \{@inheritDoc\} |

**Returns:**
布尔 - \{@inheritDoc\}
### retainAll(Collection&lt;?&gt; c) {#retainAll-java.util.Collection----}
```
public boolean retainAll(Collection<?> c)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \{@inheritDoc\} |

**Returns:**
布尔 - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


获取集合中属性的数量。

**Returns:**
int - 集合中属性的数量。
### toArray() {#toArray--}
```
public Object[] toArray()
```




**Returns:**
java.lang.Object[] - \{@inheritDoc\}
