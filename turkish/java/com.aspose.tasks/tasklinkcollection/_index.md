---
title: "TaskLinkCollection"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Nesnelerden oluşan bir koleksiyonu temsil eder."
type: docs
weight: 296
url: /tr/java/com.aspose.tasks/tasklinkcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskLinkCollection extends AbstractList<TaskLink>
```

Bir [Task](../../com.aspose.tasks/task) nesnesi koleksiyonunu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Task pred, Task succ)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-) | TaskLinkCollection nesnesine eklenmiş Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) örneğini döndürür. |
| [add(Task pred, Task succ, int linkType)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-) | TaskLinkCollection nesnesine eklenmiş [TaskLink](../../com.aspose.tasks/tasklink) örneğini döndürür. |
| [add(Task pred, Task succ, int linkType, Duration lag)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-) | TaskLinkCollection nesnesine eklenmiş [TaskLink](../../com.aspose.tasks/tasklink) örneğini döndürür. |
| [add(TaskLink e)](#add-com.aspose.tasks.TaskLink-) | Bu, yalnızca UnsupportedOperationException fırlatan ICollection'ın Add metodunun stub uygulamasıdır. |
| [clear()](#clear--) | Dahili kullanım için ayrılmıştır. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getParentProject()](#getParentProject--) | ResourceAssignmentCollection nesnesinin üst proje nesnesini alır. |
| [remove(int index)](#remove-int-) | Bu koleksiyonda belirtilen konumdaki öğeyi kaldırır ve kaldırılan öğeyi döndürür. |
| [remove(Object item)](#remove-java.lang.Object-) | Bir projeden görev bağlantısını kaldırır. |
| [size()](#size--) | Bu `TaskLinkCollection` nesnesinde bulunan nesne sayısını döndürür. |
| [sort(Comparator&lt;? super TaskLink&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--) | \{@inheritDoc\} |
| [toList()](#toList--) | TaskLinkCollection nesnesini [TaskLink](../../com.aspose.tasks/tasklink) nesnelerinin bir listesine dönüştürür. |
### add(Task pred, Task succ) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-}
```
public final TaskLink add(Task pred, Task succ)
```


TaskLinkCollection nesnesine eklenmiş Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) örneğini döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Önceki görev. |
| succ | [Task](../../com.aspose.tasks/task) | Sonraki görev. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-}
```
public final TaskLink add(Task pred, Task succ, int linkType)
```


TaskLinkCollection nesnesine eklenmiş [TaskLink](../../com.aspose.tasks/tasklink) örneğini döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Önceki görev. |
| succ | [Task](../../com.aspose.tasks/task) | Sonraki görev. |
| linkType | int | Bağlantı türü [TaskLinkType](../../com.aspose.tasks/tasklinktype) |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType, Duration lag) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-}
```
public final TaskLink add(Task pred, Task succ, int linkType, Duration lag)
```


TaskLinkCollection nesnesine eklenmiş [TaskLink](../../com.aspose.tasks/tasklink) örneğini döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Önceki görev. |
| succ | [Task](../../com.aspose.tasks/task) | Sonraki görev. |
| linkType | int | Bağlantı türü [TaskLinkType](../../com.aspose.tasks/tasklinktype) |
| lag | [Duration](../../com.aspose.tasks/duration) | Bağlantı gecikmesi [Duration](../../com.aspose.tasks/duration). |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link which has been added to this object.
### add(TaskLink e) {#add-com.aspose.tasks.TaskLink-}
```
public final boolean add(TaskLink e)
```


Bu, yalnızca UnsupportedOperationException fırlatan ICollection'ın Add metodunun stub uygulamasıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| e | [TaskLink](../../com.aspose.tasks/tasklink) | Eklenecek öğe. |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Dahili kullanım için ayrılmıştır.

### get(int index) {#get-int-}
```
public TaskLink get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - \{@inheritDoc\}
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


ResourceAssignmentCollection nesnesinin üst proje nesnesini alır.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent `Project` for this object.
### remove(int index) {#remove-int-}
```
public final TaskLink remove(int index)
```


Bu koleksiyonda belirtilen konumdaki öğeyi kaldırır ve kaldırılan öğeyi döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | öğeyi kaldırmak için belirtilen konum. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Bir projeden görev bağlantısını kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | java.lang.Object | kaldırılacak `TaskLink` sınıfının belirtilen örneği. |

**Returns:**
boolean - bu koleksiyondan kaldırılan `TaskLink` sınıfının örneğini döndürür.
### size() {#size--}
```
public final int size()
```


Bu `TaskLinkCollection` nesnesinde bulunan nesne sayısını döndürür. Salt okunur `int`.

**Returns:**
int - bu koleksiyonda bulunan nesne sayısını döndürür.
### sort(Comparator&lt;? super TaskLink&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--}
```
public void sort(Comparator<? super TaskLink> c)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.TaskLink&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<TaskLink> toList()
```


TaskLinkCollection nesnesini [TaskLink](../../com.aspose.tasks/tasklink) nesnelerinin bir listesine dönüştürür.

**Returns:**
java.util.List&lt;com.aspose.tasks.TaskLink&gt; - [TaskLink](../../com.aspose.tasks/tasklink) nesnelerinin listesi.
