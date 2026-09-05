---
title: "TaskBaseline"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "タスクのベースラインを表します。"
type: docs
weight: 291
url: /ja/java/com.aspose.tasks/taskbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)

**All Implemented Interfaces:**
java.lang.Comparable
```
public class TaskBaseline extends Baseline implements Comparable<Baseline>
```

タスクのベースラインを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [TaskBaseline(Task task)](#TaskBaseline-com.aspose.tasks.Task-) | 新しい [TaskBaseline](../../com.aspose.tasks/taskbaseline) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [compareTo(TaskBaseline other)](#compareTo-com.aspose.tasks.TaskBaseline-) | IComparable インターフェイスの実装。 |
| [equals(TaskBaseline other)](#equals-com.aspose.tasks.TaskBaseline-) | このインスタンスが指定された TaskBaseline オブジェクトと等しいかどうかを示す値を返します。 |
| [equals(Object obj)](#equals-java.lang.Object-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [getDuration()](#getDuration--) | ベースラインが保存されたときのタスクの予定期間を取得します。 |
| [getEstimatedDuration()](#getEstimatedDuration--) | タスクのベースライン期間が見積もられたかどうかを示す値を取得します。 |
| [getFinish()](#getFinish--) | ベースラインが保存されたときのタスクの予定完了日を取得します。 |
| [getFixedCost()](#getFixedCost--) | ベースラインが保存されたときのタスクの固定コストを取得します。 |
| [getInterim()](#getInterim--) | これが中間ベースラインかどうかを示す値を取得します。 |
| [getStart()](#getStart--) | ベースラインが保存されたときのタスクの予定開始日を取得します。 |
| [getTimephasedData()](#getTimephasedData--) | このオブジェクトの TimephasedDataCollection インスタンスを取得します。 |
| [hashCode()](#hashCode--) | [TaskBaseline](../../com.aspose.tasks/taskbaseline) クラスのインスタンスのハッシュコード値を返します。 |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | ベースラインが保存されたときのタスクの予定期間を設定します。 |
| [setEstimatedDuration(boolean value)](#setEstimatedDuration-boolean-) | タスクのベースライン期間が見積もられたかどうかを示す値を設定します。 |
| [setFinish(Date value)](#setFinish-java.util.Date-) | ベースラインが保存されたときのタスクの予定完了日を設定します。 |
| [setFixedCost(double value)](#setFixedCost-double-) | ベースラインが保存されたときのタスクの固定コストを設定します。 |
| [setInterim(boolean value)](#setInterim-boolean-) | これが中間ベースラインかどうかを示す値を設定します。 |
| [setStart(Date value)](#setStart-java.util.Date-) | ベースラインが保存されたときのタスクの予定開始日を設定します。 |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | このオブジェクトの TimephasedDataCollection インスタンスを設定します。 |
### TaskBaseline(Task task) {#TaskBaseline-com.aspose.tasks.Task-}
```
public TaskBaseline(Task task)
```


新しい [TaskBaseline](../../com.aspose.tasks/taskbaseline) クラスのインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | ベースラインの親タスク。 |

### compareTo(TaskBaseline other) {#compareTo-com.aspose.tasks.TaskBaseline-}
```
public final int compareTo(TaskBaseline other)
```


IComparable インターフェイスの実装です。このインスタンスを指定された Baseline オブジェクトと比較します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | このインスタンスと比較するための指定された Baseline オブジェクト。 |

**Returns:**
int - このインスタンスが指定されたオブジェクトより小さい場合は -1、指定されたオブジェクトより大きい場合は 1 を返し、それ以外の場合は 0 を返します。
### equals(TaskBaseline other) {#equals-com.aspose.tasks.TaskBaseline-}
```
public final boolean equals(TaskBaseline other)
```


このインスタンスが指定された TaskBaseline オブジェクトと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | このインスタンスと比較するための指定された AssignmentBaseline オブジェクトです。 |

**Returns:**
boolean - このインスタンスが指定された TaskBaseline オブジェクトと等しい場合は true を返し、そうでない場合は false を返します。
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
boolean - 指定されたオブジェクトがこのインスタンスと同じ UID 値を持つ TaskBaseline の場合は **True**、それ以外の場合は **false** です。
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


ベースラインが保存されたときのタスクの予定期間を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the scheduled duration of the task when the baseline was saved.
### getEstimatedDuration() {#getEstimatedDuration--}
```
public final boolean getEstimatedDuration()
```


タスクのベースライン期間が見積もられたかどうかを示す値を取得します。

**Returns:**
boolean - タスクのベースライン期間が見積もられたかどうかを示す値です。
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


ベースラインが保存されたときのタスクの予定完了日を取得します。

**Returns:**
java.util.Date - ベースラインが保存されたときのタスクの予定完了日です。
### getFixedCost() {#getFixedCost--}
```
public final double getFixedCost()
```


ベースラインが保存されたときのタスクの固定コストを取得します。

**Returns:**
double - ベースラインが保存されたときのタスクの固定コストです。
### getInterim() {#getInterim--}
```
public final boolean getInterim()
```


これが中間ベースラインかどうかを示す値を取得します。

**Returns:**
boolean - これが暫定ベースラインかどうかを示す値です。
### getStart() {#getStart--}
```
public final Date getStart()
```


ベースラインが保存されたときのタスクの予定開始日を取得します。

**Returns:**
java.util.Date - ベースラインが保存されたときのタスクの予定開始日です。
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


このオブジェクトの TimephasedDataCollection インスタンスを取得します。タスクベースラインに関連付けられた時間フェーズデータです。

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection instance for this object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


[TaskBaseline](../../com.aspose.tasks/taskbaseline) クラスのインスタンスのハッシュコード値を返します。

**Returns:**
int - このオブジェクトのハッシュコード値を返します。
### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


ベースラインが保存されたときのタスクの予定期間を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ベースラインが保存されたときのタスクの予定期間です。 |

### setEstimatedDuration(boolean value) {#setEstimatedDuration-boolean-}
```
public final void setEstimatedDuration(boolean value)
```


タスクのベースライン期間が見積もられたかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | タスクのベースライン期間が見積もりかどうかを示す値です。 |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


ベースラインが保存されたときのタスクの予定完了日を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | ベースラインが保存されたときのタスクの予定完了日です。 |

### setFixedCost(double value) {#setFixedCost-double-}
```
public final void setFixedCost(double value)
```


ベースラインが保存されたときのタスクの固定コストを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | double | ベースラインが保存されたときのタスクの固定コストです。 |

### setInterim(boolean value) {#setInterim-boolean-}
```
public final void setInterim(boolean value)
```


これが中間ベースラインかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | これが暫定ベースラインかどうかを示す値です。 |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


ベースラインが保存されたときのタスクの予定開始日を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | ベースラインが保存されたときのタスクの予定開始日です。 |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


このオブジェクトの TimephasedDataCollection インスタンスを設定します。タスクベースラインに関連付けられた時間フェーズデータです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | このオブジェクトの TimephasedDataCollection インスタンスです。 |

