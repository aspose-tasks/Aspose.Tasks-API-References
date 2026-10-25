---
title: "TaskCollection"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "オブジェクトのコレクションを表します。"
type: docs
weight: 293
url: /ja/java/com.aspose.tasks/taskcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskCollection extends AbstractList<Task>
```

[Task](../../com.aspose.tasks/task) オブジェクトのコレクションを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [add()](#add--) | 最後のタスクと同じアウトラインレベルで、プロジェクト タスク コレクションに新しいタスクを追加します。 |
| [add(RecurringTaskParameters parameters)](#add-com.aspose.tasks.RecurringTaskParameters-) | 指定された ID のタスクの前に、同じアウトラインレベルで新しいタスクを挿入します。 |
| [add(Task item)](#add-com.aspose.tasks.Task-) | 指定されたタスクを [TaskCollection](../../com.aspose.tasks/taskcollection) クラスのインスタンスに追加します。 |
| [add(String taskName)](#add-java.lang.String-) | 子タスク コレクションに新しいタスクを追加します。 |
| [add(String taskName, int beforeTaskId)](#add-java.lang.String-int-) | 子タスク コレクションに新しい繰り返しタスクを追加します。 |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Task item)](#contains-com.aspose.tasks.Task-) | コレクションが指定された項目を含むか確認します。 |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | このコレクションの親タスクが祖先である、指定された Id のタスクを返します。 |
| [getByUid(int uid)](#getByUid-int-) | このコレクションの父タスクが祖先である、指定された Uid のタスクを返します。 |
| [getParentProject()](#getParentProject--) | TaskCollection オブジェクトの親プロジェクトを取得します。 |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | このコレクションが読み取り専用かどうかを示す値を取得します。 |
| [iterator()](#iterator--) | このコレクションの列挙子を返します。 |
| [remove(Object item)](#remove-java.lang.Object-) | これは ICollection の Remove メソッドのスタブ実装で、UnsupportedOperationException をスローするだけです。 |
| [size()](#size--) | TaskCollection に含まれるオブジェクトの数を取得します。 |
| [sort(Comparator&lt;? super Task&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.Task--) | \{@inheritDoc\} |
| [toList()](#toList--) | TaskCollection オブジェクトを [Task](../../com.aspose.tasks/task) オブジェクトのリストに変換します。 |
### add() {#add--}
```
public final Task add()
```


最後のタスクと同じアウトラインレベルで、プロジェクト タスク コレクションに新しいタスクを追加します。

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(RecurringTaskParameters parameters) {#add-com.aspose.tasks.RecurringTaskParameters-}
```
public final Task add(RecurringTaskParameters parameters)
```


指定された ID のタスクの前に、同じアウトラインレベルで新しいタスクを挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| parameters | [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) | 繰り返しタスクの作成のために指定されたパラメータ。 |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(Task item) {#add-com.aspose.tasks.Task-}
```
public final boolean add(Task item)
```


[TaskCollection](../../com.aspose.tasks/taskcollection) クラスのインスタンスに指定されたタスクを追加します。ParentProject.CalculationMode が None の場合、ユーザーはこのメソッド使用後に Project.Recalculate() を呼び出す必要があります（これにより、すべてのプロジェクト タスク（開始/完了日、早期/遅延日を設定）を再スケジュールし、スラック、作業量、コスト フィールド、ID、アウトラインレベルなどの依存フィールドを計算します）。ParentProject.CalculationMode が Manual の場合、メソッドはタスク ID、アウトラインレベル、アウトライン番号のみを自動的に計算します。ParentProject.CalculationMode が Automatic の場合、メソッドはプロジェクトのすべてのタスクを自動的に再スケジュールします（開始/完了日を設定し、早期/遅延日を設定し、スラック、作業量、コスト フィールドを計算し、ID とアウトラインレベルを再計算します）。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | このタスク コレクションに追加すべき指定されたタスク。 |

**Returns:**
boolean - 操作が成功した場合は true。
### add(String taskName) {#add-java.lang.String-}
```
public final Task add(String taskName)
```


子タスク コレクションに新しいタスクを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| taskName | java.lang.String | 指定されたタスク名。 |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(String taskName, int beforeTaskId) {#add-java.lang.String-int-}
```
public final Task add(String taskName, int beforeTaskId)
```


子タスク コレクションに新しい繰り返しタスクを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| taskName | java.lang.String | 指定されたタスク名。 |
| beforeTaskId | int | 新しいタスクが挿入されるタスクの前にある、指定された ID。 |

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


コレクションが指定された項目を含むか確認します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | 確認する項目です。 |

**Returns:**
boolean - コレクションが項目を含む場合は true、そうでない場合は false。
### get(int index) {#get-int-}
```
public Task get(int index)
```


(@inheritDoc\}

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | \{@inheritDoc\} |

**Returns:**
[Task](../../com.aspose.tasks/task) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Task getById(int id)
```


このコレクションの親タスクが祖先である、指定された Id のタスクを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| id | int | TaskEntity Id |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified id whose ancestor is parent task of this collection.
### getByUid(int uid) {#getByUid-int-}
```
public final Task getByUid(int uid)
```


このコレクションの父タスクが祖先である、指定された Uid のタスクを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| uid | int | TaskEntity Uid. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified uid whose ancestor is parent task of this collection.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


TaskCollection オブジェクトの親プロジェクトを取得します。

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the TaskCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


このコレクションが読み取り専用かどうかを示す値を取得します。

**Returns:**
boolean - このコレクションが読み取り専用かどうかを示す値です。
### iterator() {#iterator--}
```
public final Iterator<Task> iterator()
```


このコレクションの列挙子を返します。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Task&gt; - このコレクションの列挙子です。
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


これは ICollection の Remove メソッドのスタブ実装で、UnsupportedOperationException をスローするだけです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| アイテム | java.lang.Object | 削除する項目。 |

**Returns:**
boolean - アイテムが削除された場合は `true`、それ以外は `false`。
### size() {#size--}
```
public final int size()
```


TaskCollection に含まれるオブジェクトの数を取得します。

**Returns:**
int - TaskCollection に含まれるオブジェクトの数です。
### sort(Comparator&lt;? super Task&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.Task--}
```
public final void sort(Comparator<? super Task> c)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.Task&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Task> toList()
```


TaskCollection オブジェクトを [Task](../../com.aspose.tasks/task) オブジェクトのリストに変換します。

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - このコレクションの [Task](../../com.aspose.tasks/task) クラスインスタンスを含むリストを返します。
