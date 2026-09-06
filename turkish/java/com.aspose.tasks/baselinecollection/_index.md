---
title: "BaselineCollection"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Nesnelerden oluşan bir koleksiyonu temsil eder."
type: docs
weight: 27
url: /tr/java/com.aspose.tasks/baselinecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class BaselineCollection extends AbstractList<Baseline>
```

[Baseline](../../com.aspose.tasks/baseline) nesnelerinin bir koleksiyonunu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Baseline item)](#add-com.aspose.tasks.Baseline-) | Bu, ICollection'ın Add metodunun taslak uygulamasıdır ve yalnızca NotSupportedException fırlatır. |
| [get(int index)](#get-int-) | Belirtilen konumdaki baseline'ı döndürür. |
| [getParentResource()](#getParentResource--) | Bu koleksiyon için üst [Resource](../../com.aspose.tasks/resource) öğesini alır. |
| [remove(int index)](#remove-int-) | Bu listedeki belirtilen konumdaki öğeyi kaldırır. |
| [remove(Object item)](#remove-java.lang.Object-) | Bu koleksiyondan temel çizgiyi kaldırır. |
| [size()](#size--) | Bu BaselineCollection nesnesinde bulunan nesne sayısını alır. |
| [toList()](#toList--) | BaselineCollection nesnesini [Baseline](../../com.aspose.tasks/baseline) nesnelerinin listesine dönüştürür. |
### add(Baseline item) {#add-com.aspose.tasks.Baseline-}
```
public final boolean add(Baseline item)
```


Bu, ICollection'ın Add metodunun taslak uygulamasıdır ve yalnızca NotSupportedException fırlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | [Baseline](../../com.aspose.tasks/baseline) | Kaldırılacak öğe. |

**Returns:**
boolean - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public Baseline get(int index)
```


Belirtilen konumdaki baseline'ı döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | döndürülecek öğenin indeksi. |

**Returns:**
[Baseline](../../com.aspose.tasks/baseline) - the baseline at the specified position.
### getParentResource() {#getParentResource--}
```
public final Resource getParentResource()
```


Bu koleksiyon için üst [Resource](../../com.aspose.tasks/resource) öğesini alır.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the parent [Resource](../../com.aspose.tasks/resource) for this collection.
### remove(int index) {#remove-int-}
```
public Baseline remove(int index)
```


Bu listedeki belirtilen konumdaki öğeyi kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Baseline](../../com.aspose.tasks/baseline) - \{@inheritDoc\}
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Bu koleksiyondan temel çizgiyi kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | java.lang.Object | Kaldırılacak [Baseline](../../com.aspose.tasks/baseline) örneği. |

**Returns:**
boolean - [Baseline](../../com.aspose.tasks/baseline) örneği başarıyla kaldırıldıysa true; aksi takdirde false
### size() {#size--}
```
public final int size()
```


Bu BaselineCollection nesnesinde bulunan nesne sayısını alır.

**Returns:**
int - bu BaselineCollection nesnesinde bulunan nesne sayısı.
### toList() {#toList--}
```
public final List<Baseline> toList()
```


BaselineCollection nesnesini [Baseline](../../com.aspose.tasks/baseline) nesnelerinin listesine dönüştürür.

**Returns:**
java.util.List&lt;com.aspose.tasks.Baseline&gt; - [Baseline](../../com.aspose.tasks/baseline) nesnelerinin listesi.
