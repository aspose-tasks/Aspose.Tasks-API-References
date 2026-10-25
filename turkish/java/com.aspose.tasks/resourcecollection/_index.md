---
title: "ResourceCollection"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Nesnelerden oluşan bir koleksiyonu temsil eder."
type: docs
weight: 251
url: /tr/java/com.aspose.tasks/resourcecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceCollection extends AbstractList<Resource>
```

Bir [Resource](../../com.aspose.tasks/resource) nesnesi koleksiyonunu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add()](#add--) | Bir proje kaynakları koleksiyonunun son konumuna yeni kaynak ekler. |
| [add(Resource e)](#add-com.aspose.tasks.Resource-) | \{@inheritDoc\} |
| [add(String resourceName)](#add-java.lang.String-) | Bir proje kaynakları koleksiyonunun son konumuna yeni kaynak ekler. |
| [add(String resourceName, int beforeResourceId)](#add-java.lang.String-int-) | Belirtilen konumda bir proje kaynakları koleksiyonuna yeni kaynak ekler. |
| [clear()](#clear--) | Doğrudan temizleme desteklenmez, bu yöntem sadece UnsupportedOperationException fırlatır. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Belirtilen kimliğe sahip bir kaynağı döndürür. |
| [getByUid(int uid)](#getByUid-int-) | Belirtilen Uid'ye sahip bir kaynağı döndürür. |
| [getParentProject()](#getParentProject--) | ResourceCollection nesnesinin üst projesini alır. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | \{@inheritDoc\} |
| [iterator()](#iterator--) | Bu koleksiyon için bir enumerator döndürür. |
| [remove(Object o)](#remove-java.lang.Object-) | Bu, Collection sınıfının remove yönteminin stub (taslak) uygulamasıdır ve sadece UnsupportedOperationException fırlatır. |
| [size()](#size--) | ResourceCollection içinde bulunan öğe sayısını alır. |
| [sort(Comparator&lt;? super Resource&gt; comparer)](#sort-java.util.Comparator---super-com.aspose.tasks.Resource--) | \{@inheritDoc\} |
| [toList()](#toList--) | ResourceCollection nesnesini [Resource](../../com.aspose.tasks/resource) nesnelerinin bir listesine dönüştürür. |
### add() {#add--}
```
public final Resource add()
```


Bir proje kaynakları koleksiyonunun son konumuna yeni kaynak ekler.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(Resource e) {#add-com.aspose.tasks.Resource-}
```
public final boolean add(Resource e)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| e | [Resource](../../com.aspose.tasks/resource) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### add(String resourceName) {#add-java.lang.String-}
```
public final Resource add(String resourceName)
```


Bir proje kaynakları koleksiyonunun son konumuna yeni kaynak ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| resourceName | java.lang.String | Bir kaynağın adı. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(String resourceName, int beforeResourceId) {#add-java.lang.String-int-}
```
public final Resource add(String resourceName, int beforeResourceId)
```


Belirtilen konumda bir proje kaynakları koleksiyonuna yeni kaynak ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| resourceName | java.lang.String | Bir kaynağın adı. |
| beforeResourceId | int | Bir proje kaynakları koleksiyonundaki önceki kaynağın konumu. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### clear() {#clear--}
```
public final void clear()
```


Doğrudan temizleme desteklenmez, bu yöntem sadece UnsupportedOperationException fırlatır.

### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public Resource get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Resource getById(int id)
```


Belirtilen kimliğe sahip bir kaynağı döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | id | int | Belirtilen kimlik. |

--------------------

O(1) karmaşıklık. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified id if present; otherwise, null.
### getByUid(int uid) {#getByUid-int-}
```
public final Resource getByUid(int uid)
```


Belirtilen Uid'ye sahip bir kaynağı döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | uid | int | Belirtilen uid. |

--------------------

O(1) karmaşıklık. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


ResourceCollection nesnesinin üst projesini alır.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```




**Returns:**
boolean - \{@inheritDoc\}
### iterator() {#iterator--}
```
public final Iterator<Resource> iterator()
```


Bu koleksiyon için bir enumerator döndürür.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Resource&gt; - bu koleksiyon için bir yineleyici.
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Bu, Collection sınıfının remove yönteminin stub (taslak) uygulamasıdır ve sadece UnsupportedOperationException fırlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | kaldırılacak öğe. |

**Returns:**
boolean - öğe kaldırıldıysa `true`; aksi takdirde `false`.
### size() {#size--}
```
public final int size()
```


ResourceCollection içinde bulunan öğe sayısını alır.

--------------------

Salt okunur `int`.

**Returns:**
int - ResourceCollection içinde bulunan öğe sayısı.
### sort(Comparator&lt;? super Resource&gt; comparer) {#sort-java.util.Comparator---super-com.aspose.tasks.Resource--}
```
public final void sort(Comparator<? super Resource> comparer)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| comparer | java.util.Comparator&lt;? super com.aspose.tasks.Resource&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Resource> toList()
```


ResourceCollection nesnesini [Resource](../../com.aspose.tasks/resource) nesnelerinin bir listesine dönüştürür.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - [Resource](../../com.aspose.tasks/resource) nesnelerinin Listesi.
