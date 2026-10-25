---
title: "TaskLinkCollection"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "オブジェクトのコレクションを表します。"
type: docs
weight: 296
url: /ja/java/com.aspose.tasks/tasklinkcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskLinkCollection extends AbstractList<TaskLink>
```

[Task](../../com.aspose.tasks/task) オブジェクトのコレクションを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [add(Task pred, Task succ)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-) | TaskLinkCollection オブジェクトに追加された、Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) のインスタンスを返します。 |
| [add(Task pred, Task succ, int linkType)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-) | TaskLinkCollection オブジェクトに追加された、[TaskLink](../../com.aspose.tasks/tasklink) のインスタンスを返します。 |
| [add(Task pred, Task succ, int linkType, Duration lag)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-) | TaskLinkCollection オブジェクトに追加された、[TaskLink](../../com.aspose.tasks/tasklink) のインスタンスを返します。 |
| [add(TaskLink e)](#add-com.aspose.tasks.TaskLink-) | これは ICollection の Add メソッドのスタブ実装で、UnsupportedOperationException をスローするだけです。 |
| [clear()](#clear--) | 内部使用のために予約されています。 |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getParentProject()](#getParentProject--) | ResourceAssignmentCollection オブジェクトの親プロジェクトを取得します。 |
| [remove(int index)](#remove-int-) | このコレクション内の指定された位置にある要素を削除し、削除された要素を返します。 |
| [remove(Object item)](#remove-java.lang.Object-) | プロジェクトからタスクリンクを削除します。 |
| [size()](#size--) | この `TaskLinkCollection` オブジェクトに含まれるオブジェクト数を返します。 |
| [sort(Comparator&lt;? super TaskLink&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--) | \{@inheritDoc\} |
| [toList()](#toList--) | TaskLinkCollection オブジェクトを [TaskLink](../../com.aspose.tasks/tasklink) オブジェクトのリストに変換します。 |
### add(Task pred, Task succ) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-}
```
public final TaskLink add(Task pred, Task succ)
```


TaskLinkCollection オブジェクトに追加された、Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) のインスタンスを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | 先行タスク。 |
| succ | [Task](../../com.aspose.tasks/task) | 後続タスク。 |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-}
```
public final TaskLink add(Task pred, Task succ, int linkType)
```


TaskLinkCollection オブジェクトに追加された、[TaskLink](../../com.aspose.tasks/tasklink) のインスタンスを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | 先行タスク。 |
| succ | [Task](../../com.aspose.tasks/task) | 後続タスク。 |
| linkType | int | リンクタイプ [TaskLinkType](../../com.aspose.tasks/tasklinktype) |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType, Duration lag) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-}
```
public final TaskLink add(Task pred, Task succ, int linkType, Duration lag)
```


TaskLinkCollection オブジェクトに追加された、[TaskLink](../../com.aspose.tasks/tasklink) のインスタンスを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | 先行タスク。 |
| succ | [Task](../../com.aspose.tasks/task) | 後続タスク。 |
| linkType | int | リンクタイプ [TaskLinkType](../../com.aspose.tasks/tasklinktype) |
| lag | [Duration](../../com.aspose.tasks/duration) | リンク遅延 [Duration](../../com.aspose.tasks/duration)。 |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link which has been added to this object.
### add(TaskLink e) {#add-com.aspose.tasks.TaskLink-}
```
public final boolean add(TaskLink e)
```


これは ICollection の Add メソッドのスタブ実装で、UnsupportedOperationException をスローするだけです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| e | [TaskLink](../../com.aspose.tasks/tasklink) | 追加する項目。 |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


内部使用のために予約されています。

### get(int index) {#get-int-}
```
public TaskLink get(int index)
```


(@inheritDoc\}

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | \{@inheritDoc\} |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - \{@inheritDoc\}
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


ResourceAssignmentCollection オブジェクトの親プロジェクトを取得します。

**Returns:**
[Project](../../com.aspose.tasks/project) - parent `Project` for this object.
### remove(int index) {#remove-int-}
```
public final TaskLink remove(int index)
```


このコレクション内の指定された位置にある要素を削除し、削除された要素を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 要素を削除する指定された位置。 |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


プロジェクトからタスクリンクを削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| アイテム | java.lang.Object | 削除するための `TaskLink` クラスの指定されたインスタンス。 |

**Returns:**
boolean - このコレクションから削除された `TaskLink` クラスのインスタンスを返します。
### size() {#size--}
```
public final int size()
```


この `TaskLinkCollection` オブジェクトに含まれるオブジェクト数を返します。読み取り専用 `int`。

**Returns:**
int - このコレクションに含まれるオブジェクト数を返します。
### sort(Comparator&lt;? super TaskLink&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--}
```
public void sort(Comparator<? super TaskLink> c)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.TaskLink&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<TaskLink> toList()
```


TaskLinkCollection オブジェクトを [TaskLink](../../com.aspose.tasks/tasklink) オブジェクトのリストに変換します。

**Returns:**
java.util.List&lt;com.aspose.tasks.TaskLink&gt; - [TaskLink](../../com.aspose.tasks/tasklink) オブジェクトのリスト。
