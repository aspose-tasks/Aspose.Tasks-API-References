---
title: "TaskLink"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "前任タスクへのリンクを表します。"
type: docs
weight: 295
url: /ja/java/com.aspose.tasks/tasklink/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public final class TaskLink implements System.IEquatable<TaskLink>
```

前任タスクへのリンクを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [equals(TaskLink other)](#equals-com.aspose.tasks.TaskLink-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [equals(Object obj)](#equals-java.lang.Object-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [getCrossProjectName()](#getCrossProjectName--) | 外部の前任プロジェクトを取得します。 |
| [getLagFormat()](#getLagFormat--) | 遅延形式を表すフォーマットを取得します。 |
| [getLinkLag()](#getLinkLag--) | 遅延を 0.1 分単位またはパーセンテージで取得します。 |
| [getLinkLagTimeSpan()](#getLinkLagTimeSpan--) | LagFormat に応じて遅延期間を取得します。 |
| [getLinkType()](#getLinkType--) | リンクのタイプを取得します。 |
| [getPredTask()](#getPredTask--) | 前任タスクを取得します。 |
| [getSuccTask()](#getSuccTask--) | 後続タスクを取得します。 |
| [hashCode()](#hashCode--) | [TaskLink](../../com.aspose.tasks/tasklink) クラスのインスタンスに対するハッシュコード値を返します。 |
| [isCrossProject()](#isCrossProject--) | 前任タスクが別のプロジェクトの一部であるかどうかを示す値を取得します。 |
| [setCrossProject(boolean value)](#setCrossProject-boolean-) | 前任タスクが別のプロジェクトの一部であるかどうかを示す値を設定します。 |
| [setCrossProjectName(String value)](#setCrossProjectName-java.lang.String-) | 外部の前任プロジェクトを設定します。 |
| [setLagFormat(byte value)](#setLagFormat-byte-) | 遅延フォーマットを表す形式を設定します。 |
| [setLinkLag(int value)](#setLinkLag-int-) | 遅延を1分の10単位またはパーセンテージで設定します。 |
| [setLinkLagTimeSpan(double value)](#setLinkLagTimeSpan-double-) | LagFormat に応じて遅延期間を設定します。 |
| [setLinkType(int value)](#setLinkType-int-) | リンクのタイプを設定します。 |
| [setPredTask(Task value)](#setPredTask-com.aspose.tasks.Task-) | 前任タスクを設定します。 |
| [setSuccTask(Task value)](#setSuccTask-com.aspose.tasks.Task-) | 後続タスクを設定します。 |
| [toString()](#toString--) | TaskLink の文字列表現を返します。 |
### equals(TaskLink other) {#equals-com.aspose.tasks.TaskLink-}
```
public final boolean equals(TaskLink other)
```


このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [TaskLink](../../com.aspose.tasks/tasklink) | このインスタンスと比較するための、指定された [TaskLink](../../com.aspose.tasks/tasklink) クラスのインスタンス。 |

**Returns:**
boolean - 指定された [TaskLink](../../com.aspose.tasks/tasklink) クラスのインスタンスがこのインスタンスと同じ前任タスクと後続タスクを持つ場合は **True**、それ以外の場合は **false**。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj | java.lang.Object | このインスタンスと比較するオブジェクトです。 |

**Returns:**
boolean - 指定されたオブジェクトがこのインスタンスと同じ前任タスクと後続タスクを持つ TaskLink である場合は **True**、それ以外の場合は **false**。
### getCrossProjectName() {#getCrossProjectName--}
```
public final String getCrossProjectName()
```


外部の前任プロジェクトを取得します。

**Returns:**
java.lang.String - 外部の前任プロジェクト。
### getLagFormat() {#getLagFormat--}
```
public final byte getLagFormat()
```


遅延形式を表すフォーマットを取得します。

**Returns:**
byte - 遅延フォーマットを表す形式。
### getLinkLag() {#getLinkLag--}
```
public final int getLinkLag()
```


遅延を 0.1 分単位またはパーセンテージで取得します。

**Returns:**
int - 1分の10単位またはパーセンテージでの遅延。
### getLinkLagTimeSpan() {#getLinkLagTimeSpan--}
```
public final double getLinkLagTimeSpan()
```


LagFormat に応じて遅延期間を取得します。

**Returns:**
double - LagFormat に応じた遅延期間。
### getLinkType() {#getLinkType--}
```
public final int getLinkType()
```


リンクのタイプを取得します。

**Returns:**
int - リンクのタイプ。
### getPredTask() {#getPredTask--}
```
public final Task getPredTask()
```


前任タスクを取得します。

**Returns:**
[Task](../../com.aspose.tasks/task) - the predecessor task.
### getSuccTask() {#getSuccTask--}
```
public final Task getSuccTask()
```


後続タスクを取得します。

**Returns:**
[Task](../../com.aspose.tasks/task) - the successor task.
### hashCode() {#hashCode--}
```
public int hashCode()
```


[TaskLink](../../com.aspose.tasks/tasklink) クラスのインスタンスに対するハッシュコード値を返します。

**Returns:**
int - このオブジェクトのハッシュコード値を返します。
### isCrossProject() {#isCrossProject--}
```
public final boolean isCrossProject()
```


前任タスクが別のプロジェクトの一部であるかどうかを示す値を取得します。

**Returns:**
boolean - 前任タスクが別のプロジェクトの一部であるかどうかを示す値。
### setCrossProject(boolean value) {#setCrossProject-boolean-}
```
public final void setCrossProject(boolean value)
```


前任タスクが別のプロジェクトの一部であるかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 前任タスクが別のプロジェクトの一部であるかどうかを示す値。 |

### setCrossProjectName(String value) {#setCrossProjectName-java.lang.String-}
```
public final void setCrossProjectName(String value)
```


外部の前任プロジェクトを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 外部の前任プロジェクト。 |

### setLagFormat(byte value) {#setLagFormat-byte-}
```
public final void setLagFormat(byte value)
```


遅延フォーマットを表す形式を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | バイト | 遅延形式を表すフォーマット。 |

### setLinkLag(int value) {#setLinkLag-int-}
```
public final void setLinkLag(int value)
```


遅延を1分の10単位またはパーセンテージで設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 遅延は1分の10単位またはパーセンテージです。 |

### setLinkLagTimeSpan(double value) {#setLinkLagTimeSpan-double-}
```
public final void setLinkLagTimeSpan(double value)
```


LagFormat に応じて遅延期間を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | 遅延期間は LagFormat に依存します。 |

### setLinkType(int value) {#setLinkType-int-}
```
public final void setLinkType(int value)
```


リンクのタイプを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | リンクのタイプ。 |

### setPredTask(Task value) {#setPredTask-com.aspose.tasks.Task-}
```
public final void setPredTask(Task value)
```


前任タスクを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | 前任タスク。 |

### setSuccTask(Task value) {#setSuccTask-com.aspose.tasks.Task-}
```
public final void setSuccTask(Task value)
```


後続タスクを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | 後続タスク。 |

### toString() {#toString--}
```
public String toString()
```


TaskLink の文字列表現を返します。表現の正確な詳細は未定義で、変更される可能性があります。

**Returns:**
java.lang.String - TaskLink オブジェクトを表す文字列。
