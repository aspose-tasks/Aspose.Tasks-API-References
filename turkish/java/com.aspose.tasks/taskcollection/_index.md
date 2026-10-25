---
title: "TaskCollection"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Nesnelerden oluşan bir koleksiyonu temsil eder."
type: docs
weight: 293
url: /tr/java/com.aspose.tasks/taskcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskCollection extends AbstractList<Task>
```

Bir [Task](../../com.aspose.tasks/task) nesnesi koleksiyonunu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add()](#add--) | Son görevin aynı taslak seviyesinde proje görevleri koleksiyonuna yeni görev ekler. |
| [add(RecurringTaskParameters parameters)](#add-com.aspose.tasks.RecurringTaskParameters-) | Belirtilen kimliğe sahip görevin önüne ve aynı taslak seviyesinde yeni bir görev ekler. |
| [add(Task item)](#add-com.aspose.tasks.Task-) | Belirtilen görevi [TaskCollection](../../com.aspose.tasks/taskcollection) sınıfının örneğine ekler. |
| [add(String taskName)](#add-java.lang.String-) | Alt görevler koleksiyonuna yeni bir görev ekler. |
| [add(String taskName, int beforeTaskId)](#add-java.lang.String-int-) | Alt görevler koleksiyonuna yeni yinelenen bir görev ekler. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Task item)](#contains-com.aspose.tasks.Task-) | Koleksiyonun belirtilen öğeyi içerip içermediğini kontrol eder. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Belirtilen Id'ye sahip ve bu koleksiyonun üst görevinin altı olan bir görevi döndürür. |
| [getByUid(int uid)](#getByUid-int-) | Belirtilen Uid'ye sahip ve bu koleksiyonun üst görevinin altı olan bir görevi döndürür. |
| [getParentProject()](#getParentProject--) | TaskCollection nesnesinin üst proje nesnesini alır. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Bu koleksiyonun yalnızca okunabilir olup olmadığını gösteren bir değeri alır. |
| [iterator()](#iterator--) | Bu koleksiyon için bir enumerator döndürür. |
| [remove(Object item)](#remove-java.lang.Object-) | Bu, yalnızca UnsupportedOperationException fırlatan ICollection'ın Remove metodunun taslak uygulamasıdır. |
| [size()](#size--) | TaskCollection içinde bulunan nesne sayısını alır. |
| [sort(Comparator&lt;? super Task&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.Task--) | \{@inheritDoc\} |
| [toList()](#toList--) | TaskCollection nesnesini [Task](../../com.aspose.tasks/task) nesnelerinin listesine dönüştürür. |
### add() {#add--}
```
public final Task add()
```


Son görevin aynı taslak seviyesinde proje görevleri koleksiyonuna yeni görev ekler.

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(RecurringTaskParameters parameters) {#add-com.aspose.tasks.RecurringTaskParameters-}
```
public final Task add(RecurringTaskParameters parameters)
```


Belirtilen kimliğe sahip görevin önüne ve aynı taslak seviyesinde yeni bir görev ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| parameters | [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) | Yinelenen görev oluşturmak için belirtilen parametreler. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(Task item) {#add-com.aspose.tasks.Task-}
```
public final boolean add(Task item)
```


Belirtilen görevi [TaskCollection](../../com.aspose.tasks/taskcollection) sınıfının örneğine ekleyin. ParentProject.CalculationMode None ise, bu yöntemi kullandıktan sonra kullanıcı Project.Recalculate() metodunu çağırmalıdır (Bu, tüm proje görevlerini (başlangıç/bitiş tarihlerini, erken/geç tarihleri ayarlar) yeniden zamanlayacak ve gecikmeler, iş ve maliyet alanları, kimlikler ve taslak seviyeleri gibi bağımlı alanları hesaplayacaktır). ParentProject.CalculationMode Manual ise yöntem yalnızca görev kimliğini, taslak seviyesini ve taslak numaralarını otomatik olarak hesaplayacaktır. ParentProject.CalculationMode Automatic ise yöntem tüm projenin görevlerini otomatik olarak yeniden zamanlayacaktır (başlangıç/bitiş tarihleri, erken/geç tarihleri ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar, kimlikleri ve taslak seviyelerini yeniden hesaplar).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | bu görev koleksiyonuna eklenmesi gereken belirtilen görev. |

**Returns:**
boolean - işlem başarılıysa true.
### add(String taskName) {#add-java.lang.String-}
```
public final Task add(String taskName)
```


Alt görevler koleksiyonuna yeni bir görev ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| taskName | java.lang.String | belirtilen görev adı. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(String taskName, int beforeTaskId) {#add-java.lang.String-int-}
```
public final Task add(String taskName, int beforeTaskId)
```


Alt görevler koleksiyonuna yeni yinelenen bir görev ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| taskName | java.lang.String | belirtilen görev adı. |
| beforeTaskId | int | Yeni bir görevin ekleneceği görevin öncesindeki belirtilen görev kimliği. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns a task which was inserted before a task with the specified id.
### clear() {#clear--}
```
public final void clear()
```




### contains(Task item) {#contains-com.aspose.tasks.Task-}
```
public final boolean contains(Task item)
```


Koleksiyonun belirtilen öğeyi içerip içermediğini kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | Kontrol edilecek öğe. |

**Returns:**
boolean - koleksiyon bir öğe içeriyorsa true, aksi takdirde false.
### get(int index) {#get-int-}
```
public Task get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Task](../../com.aspose.tasks/task) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Task getById(int id)
```


Belirtilen Id'ye sahip ve bu koleksiyonun üst görevinin altı olan bir görevi döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| id | int | TaskEntity Id |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified id whose ancestor is parent task of this collection.
### getByUid(int uid) {#getByUid-int-}
```
public final Task getByUid(int uid)
```


Belirtilen Uid'ye sahip ve bu koleksiyonun üst görevinin altı olan bir görevi döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | int | TaskEntity Uid. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified uid whose ancestor is parent task of this collection.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


TaskCollection nesnesinin üst proje nesnesini alır.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the TaskCollection object.
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
public final Iterator<Task> iterator()
```


Bu koleksiyon için bir enumerator döndürür.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Task&gt; - bu koleksiyon için bir yineleyici.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Bu, yalnızca UnsupportedOperationException fırlatan ICollection'ın Remove metodunun taslak uygulamasıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | java.lang.Object | Kaldırılacak öğe. |

**Returns:**
boolean - öğe kaldırıldıysa `true`; aksi takdirde `false`.
### size() {#size--}
```
public final int size()
```


TaskCollection içinde bulunan nesne sayısını alır.

**Returns:**
int - TaskCollection içinde bulunan nesne sayısı.
### sort(Comparator&lt;? super Task&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.Task--}
```
public final void sort(Comparator<? super Task> c)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.Task&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Task> toList()
```


TaskCollection nesnesini [Task](../../com.aspose.tasks/task) nesnelerinin listesine dönüştürür.

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - bu koleksiyonun [Task](../../com.aspose.tasks/task) sınıfı örneklerini içeren bir liste döndürür.
