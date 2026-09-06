---
title: "ResourceAssignmentCollection"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Nesnelerden oluşan bir koleksiyonu temsil eder."
type: docs
weight: 250
url: /tr/java/com.aspose.tasks/resourceassignmentcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceAssignmentCollection extends AbstractList<ResourceAssignment>
```

[ResourceAssignment](../../com.aspose.tasks/resourceassignment) nesnelerinin bir koleksiyonunu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(ResourceAssignment item)](#add-com.aspose.tasks.ResourceAssignment-) | Bu, yalnızca UnsupportedOperationException fırlatan ICollection'ın Add metodunun stub uygulamasıdır. |
| [add(Task task, Resource resource)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-) | Yeni atamayı ResourceAssignmentCollection'a ekler. |
| [add(Task task, Resource resource, double units)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-) | Yeni atamayı ResourceAssignmentCollection'a ekler. |
| [add(Task task, Resource resource, BigDecimal cost)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-) | Yeni atamayı ResourceAssignmentCollection'a ekler. |
| [clear()](#clear--) | Koleksiyondaki tüm öğeleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByUid(int uid)](#getByUid-int-) | Belirtilen uid'ye sahip bir atamayı döndürür. |
| [getParentProject()](#getParentProject--) | ResourceAssignmentCollection nesnesinin üst proje nesnesini alır. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Bu koleksiyonun yalnızca okunabilir olup olmadığını gösteren bir değeri alır. |
| [iterator()](#iterator--) | Bu koleksiyon için bir enumerator döndürür. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | Koleksiyondan belirtilen atamayı kaldırır, eğer koleksiyon yalnızca okunabilir değilse, aksi takdirde UnsupportedOperationException fırlatır. |
| [size()](#size--) | ResourceAssignmentCollection içinde bulunan nesne sayısını alır. |
| [toList()](#toList--) | ResourceAssignmentCollection nesnesini [ResourceAssignment](../../com.aspose.tasks/resourceassignment) nesnelerinin bir listesine dönüştürür. |
### add(ResourceAssignment item) {#add-com.aspose.tasks.ResourceAssignment-}
```
public final boolean add(ResourceAssignment item)
```


Bu, yalnızca UnsupportedOperationException fırlatan ICollection'ın Add metodunun stub uygulamasıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Kaldırılacak öğe. |

**Returns:**
boolean - \{@inheritDoc\}
### add(Task task, Resource resource) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-}
```
public final ResourceAssignment add(Task task, Resource resource)
```


Yeni atamayı ResourceAssignmentCollection'a ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Atanacak bir görev. |
| resource | [Resource](../../com.aspose.tasks/resource) | Atanacak bir kaynak. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, double units) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-}
```
public final ResourceAssignment add(Task task, Resource resource, double units)
```


Yeni atamayı ResourceAssignmentCollection'a ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Atanacak bir görev. |
| resource | [Resource](../../com.aspose.tasks/resource) | Atanacak bir kaynak. |
| birimler | double | Yeni atama için birim sayısı. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, BigDecimal cost) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-}
```
public final ResourceAssignment add(Task task, Resource resource, BigDecimal cost)
```


Yeni atamayı ResourceAssignmentCollection'a ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Atanacak bir görev. |
| resource | [Resource](../../com.aspose.tasks/resource) | Atanacak bir maliyet kaynağı. |
| maliyet | java.math.BigDecimal | Yeni atama için maliyet. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### clear() {#clear--}
```
public void clear()
```


Koleksiyondaki tüm öğeleri kaldırır.

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
public ResourceAssignment get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### getByUid(int uid) {#getByUid-int-}
```
public final ResourceAssignment getByUid(int uid)
```


Belirtilen uid'ye sahip bir atamayı döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | uid | int | Belirtilen uid. |

--------------------

O(1) karmaşıklık. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - ResourceAssignment with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


ResourceAssignmentCollection nesnesinin üst proje nesnesini alır.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceAssignmentCollection object.
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


Bu koleksiyonun yalnızca okunabilir olup olmadığını gösteren bir değeri alır.

**Returns:**
boolean - bu koleksiyonun yalnızca okunabilir olup olmadığını gösteren bir değer.
### iterator() {#iterator--}
```
public final Iterator<ResourceAssignment> iterator()
```


Bu koleksiyon için bir enumerator döndürür.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ResourceAssignment&gt; - bu koleksiyon için bir enumeratör.
### remove(int index) {#remove-int-}
```
public ResourceAssignment remove(int index)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Koleksiyondan belirtilen atamayı kaldırır, eğer koleksiyon yalnızca okunabilir değilse, aksi takdirde UnsupportedOperationException fırlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | Kaldırılacak atama. |

**Returns:**
boolean - true, eğer belirtilen öğe kaldırıldıysa, aksi takdirde false.
### size() {#size--}
```
public final int size()
```


ResourceAssignmentCollection içinde bulunan nesne sayısını alır.

**Returns:**
int - ResourceAssignmentCollection içinde bulunan nesne sayısı.
### toList() {#toList--}
```
public final List<ResourceAssignment> toList()
```


ResourceAssignmentCollection nesnesini [ResourceAssignment](../../com.aspose.tasks/resourceassignment) nesnelerinin bir listesine dönüştürür.

**Returns:**
java.util.List&lt;com.aspose.tasks.ResourceAssignment&gt; - [ResourceAssignment](../../com.aspose.tasks/resourceassignment) nesnelerinin listesi.
