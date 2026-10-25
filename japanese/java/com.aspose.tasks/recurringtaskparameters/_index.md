---
title: "RecurringTaskParameters"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクト内で繰り返しタスクを作成するために使用されるパラメータのセットを表します。"
type: docs
weight: 245
url: /ja/java/com.aspose.tasks/recurringtaskparameters/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskParameters
```

プロジェクト内で繰り返しタスクを作成するために使用されるパラメータのセットを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [RecurringTaskParameters()](#RecurringTaskParameters--) | 新しい [RecurringTaskParameters](../../com.aspose/tasks/recurringtaskparameters) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDuration()](#getDuration--) | 繰り返しタスクの 1 回の発生の期間を取得します。 |
| [getIgnoreResourceCalendar()](#getIgnoreResourceCalendar--) | リソースが利用可能であっても、繰り返しタスクが発生しない場合にスケジュールするかどうかを示す値を取得します。 |
| [getRecurrencePattern()](#getRecurrencePattern--) | 繰り返しタスクの再発パターンを取得します。 |
| [getTaskName()](#getTaskName--) | 繰り返しタスクの名前を取得します。 |
| [setCalendar(Project project, String calendarName)](#setCalendar-com.aspose.tasks.Project-java.lang.String-) | 繰り返しタスクのカレンダーを設定します。 |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | 繰り返しタスクの 1 回の発生の期間を設定します。 |
| [setIgnoreResourceCalendar(boolean value)](#setIgnoreResourceCalendar-boolean-) | リソースが利用可能であっても、繰り返しタスクが発生しない場合にスケジュールするかどうかを示す値を設定します。 |
| [setRecurrencePattern(RecurrencePatternBase value)](#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-) | 繰り返しタスクの再発パターンを設定します。 |
| [setTaskName(String value)](#setTaskName-java.lang.String-) | 繰り返しタスクの名前を設定します。 |
### RecurringTaskParameters() {#RecurringTaskParameters--}
```
public RecurringTaskParameters()
```


新しい [RecurringTaskParameters](../../com.aspose/tasks/recurringtaskparameters) クラスのインスタンスを初期化します。

### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


繰り返しタスクの 1 回の発生の期間を取得します。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - The instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) class.
### getIgnoreResourceCalendar() {#getIgnoreResourceCalendar--}
```
public final boolean getIgnoreResourceCalendar()
```


リソースが利用可能であっても、繰り返しタスクが発生しない場合にスケジュールするかどうかを示す値を取得します。

**Returns:**
boolean - リソースが利用可能であっても、繰り返しタスクが発生しない場合にスケジュールするかどうかを示す値。
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final RecurrencePatternBase getRecurrencePattern()
```


繰り返しタスクの再発パターンを取得します。

--------------------

`RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) 列挙体の値のいずれかになる可能性があります。

**Returns:**
[RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) - the recurrence pattern of the recurring task.
### getTaskName() {#getTaskName--}
```
public final String getTaskName()
```


繰り返しタスクの名前を取得します。

**Returns:**
java.lang.String - 繰り返しタスクの名前。
### setCalendar(Project project, String calendarName) {#setCalendar-com.aspose.tasks.Project-java.lang.String-}
```
public final void setCalendar(Project project, String calendarName)
```


繰り返しタスクのカレンダーを設定します。カレンダーはプロジェクトのカレンダーコレクションから選択されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | カレンダーコレクションを含むプロジェクト。 |
| calendarName | java.lang.String | カレンダーの名前。 |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


繰り返しタスクの 1 回の発生の期間を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) クラスのインスタンスです。 |

### setIgnoreResourceCalendar(boolean value) {#setIgnoreResourceCalendar-boolean-}
```
public final void setIgnoreResourceCalendar(boolean value)
```


リソースが利用可能であっても、繰り返しタスクが発生しない場合にスケジュールするかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | リソースが利用可能であっても、繰り返しタスクが発生しない場合にスケジュールするかどうかを示す値。 |

### setRecurrencePattern(RecurrencePatternBase value) {#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-}
```
public final void setRecurrencePattern(RecurrencePatternBase value)
```


繰り返しタスクの再発パターンを設定します。

--------------------

`RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) 列挙体の値のいずれかになる可能性があります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) | 繰り返しタスクの再発パターン。 |

### setTaskName(String value) {#setTaskName-java.lang.String-}
```
public final void setTaskName(String value)
```


繰り返しタスクの名前を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 繰り返しタスクの名前。 |

