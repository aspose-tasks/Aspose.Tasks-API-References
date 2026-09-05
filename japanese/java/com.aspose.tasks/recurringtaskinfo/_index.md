---
title: "RecurringTaskInfo"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロジェクト内の繰り返しタスクの詳細を表します。"
type: docs
weight: 244
url: /ja/java/com.aspose.tasks/recurringtaskinfo/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskInfo
```

プロジェクト内の繰り返しタスクの詳細を表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDailyRepetitions()](#getDailyRepetitions--) | 日次繰り返しパターンの繰り返し回数を取得します。 |
| [getDailyUseWorkdays()](#getDailyUseWorkdays--) | 日次繰り返しパターンで稼働日を使用するかどうかを示す値を取得します。 |
| [getDuration()](#getDuration--) | 繰り返しタスクの 1 回の発生の期間を取得します。 |
| [getEndDate()](#getEndDate--) | 発生が終了する日付を取得します。 |
| [getMonthlyDay()](#getMonthlyDay--) | 月次繰り返しパターンの日数を取得します。 |
| [getMonthlyOrdinalDay()](#getMonthlyOrdinalDay--) | 序数日を使用する場合の月次繰り返しパターンの日を取得します。 |
| [getMonthlyOrdinalNumber()](#getMonthlyOrdinalNumber--) | 月次繰り返しパターンの序数を取得します。 |
| [getMonthlyOrdinalRepetitions()](#getMonthlyOrdinalRepetitions--) | 序数日を使用する場合の月次繰り返しパターンの繰り返し回数を取得します。 |
| [getMonthlyRepetitions()](#getMonthlyRepetitions--) | 月次繰り返しパターンの繰り返し回数を取得します。 |
| [getMonthlyUseOrdinalDay()](#getMonthlyUseOrdinalDay--) | 月次繰り返しパターンで序数日を使用するかどうかを示す値を取得します。 |
| [getOccurrences()](#getOccurrences--) | 繰り返しタスクの発生回数を取得します。 |
| [getRecurrencePattern()](#getRecurrencePattern--) | 繰り返しタスクの繰り返しパターンを取得します。 |
| [getStartDate()](#getStartDate--) | 発生が開始する日付を取得します。 |
| [getTask()](#getTask--) | このインスタンスの [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) クラスの親タスクを取得します。 |
| [getUseEndDate()](#getUseEndDate--) | 繰り返しタスクで終了日または発生回数のいずれかを使用するかどうかを示す値を取得します。 |
| [getWeeklyDays()](#getWeeklyDays--) | 週次繰り返しパターンで使用される日のコレクションを取得します。 |
| [getWeeklyRepetitions()](#getWeeklyRepetitions--) | 週次繰り返しパターンの繰り返し回数を取得します。 |
| [getYearlyDate()](#getYearlyDate--) | 年次繰り返しパターンの日付を取得します。 |
| [getYearlyOrdinalDay()](#getYearlyOrdinalDay--) | 序数日を使用する場合の年次繰り返しパターンの曜日を取得します。 |
| [getYearlyOrdinalMonth()](#getYearlyOrdinalMonth--) | 序数日を使用する場合の年次繰り返しパターンの月を取得します。 |
| [getYearlyOrdinalNumber()](#getYearlyOrdinalNumber--) | 年次繰り返しパターンの序数を取得します。 |
| [getYearlyUseOrdinalDay()](#getYearlyUseOrdinalDay--) | 年次繰り返しパターンで序数日を使用するかどうかを示す値を取得します。 |
| [setDailyRepetitions(int value)](#setDailyRepetitions-int-) | 日次繰り返しパターンの繰り返し回数を設定します。 |
| [setDailyUseWorkdays(boolean value)](#setDailyUseWorkdays-boolean-) | 日次繰り返しパターンで営業日を使用するかどうかを示す値を設定します。 |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | 繰り返しタスクの 1 回の発生の期間を設定します。 |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | 発生が終了する日付を設定します。 |
| [setMonthlyDay(int value)](#setMonthlyDay-int-) | 月次繰り返しパターンの日数を設定します。 |
| [setMonthlyOrdinalDay(int value)](#setMonthlyOrdinalDay-int-) | 序数日を使用する場合の月次繰り返しパターンの日を設定します。 |
| [setMonthlyOrdinalNumber(int value)](#setMonthlyOrdinalNumber-int-) | 月次繰り返しパターンの序数を設定します。 |
| [setMonthlyOrdinalRepetitions(int value)](#setMonthlyOrdinalRepetitions-int-) | 序数日を使用する場合の月次繰り返しパターンの繰り返し回数を設定します。 |
| [setMonthlyRepetitions(int value)](#setMonthlyRepetitions-int-) | 月次繰り返しパターンの繰り返し回数を設定します。 |
| [setMonthlyUseOrdinalDay(boolean value)](#setMonthlyUseOrdinalDay-boolean-) | 月次繰り返しパターンで序数日を使用するかどうかを示す値を設定します。 |
| [setOccurrences(int value)](#setOccurrences-int-) | 定期タスクの発生回数を設定します。 |
| [setRecurrencePattern(int value)](#setRecurrencePattern-int-) | 定期タスクの繰り返しパターンを設定します。 |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | 発生開始日を設定します。 |
| [setUseEndDate(boolean value)](#setUseEndDate-boolean-) | 定期タスクで終了日を使用するか、発生回数を使用するかを示す値を設定します。 |
| [setWeeklyDays(int value)](#setWeeklyDays-int-) | 週次繰り返しパターンで使用される曜日のコレクションを設定します。 |
| [setWeeklyRepetitions(int value)](#setWeeklyRepetitions-int-) | 週次繰り返しパターンの繰り返し回数を設定します。 |
| [setYearlyDate(Date value)](#setYearlyDate-java.util.Date-) | 年次繰り返しパターンの日付を設定します。 |
| [setYearlyOrdinalDay(int value)](#setYearlyOrdinalDay-int-) | 序数日を使用する場合の年次繰り返しパターンの曜日を設定します。 |
| [setYearlyOrdinalMonth(int value)](#setYearlyOrdinalMonth-int-) | 序数日を使用する場合の年次繰り返しパターンの月を設定します。 |
| [setYearlyOrdinalNumber(int value)](#setYearlyOrdinalNumber-int-) | 年次繰り返しパターンの序数を設定します。 |
| [setYearlyUseOrdinalDay(boolean value)](#setYearlyUseOrdinalDay-boolean-) | 年次繰り返しパターンで序数日を使用するかどうかを示す値を設定します。 |
### getDailyRepetitions() {#getDailyRepetitions--}
```
public final int getDailyRepetitions()
```


日次繰り返しパターンの繰り返し回数を取得します。

**Returns:**
int - 日次繰り返しパターンの繰り返し回数。
### getDailyUseWorkdays() {#getDailyUseWorkdays--}
```
public final boolean getDailyUseWorkdays()
```


日次繰り返しパターンで稼働日を使用するかどうかを示す値を取得します。

**Returns:**
boolean - 日次繰り返しパターンで平日を使用するかどうかを示す値。
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


繰り返しタスクの 1 回の発生の期間を取得します。

--------------------

`Duration` クラスのインスタンス([getDuration()](../../com.aspose/tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose/tasks/recurringtaskinfo\#setDuration-Duration-))。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration for one occurrence of the recurring task.
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


発生が終了する日付を取得します。

**Returns:**
java.util.Date - 発生終了日。
### getMonthlyDay() {#getMonthlyDay--}
```
public final int getMonthlyDay()
```


月次繰り返しパターンの日数を取得します。

**Returns:**
int - 月次繰り返しパターンの日数。
### getMonthlyOrdinalDay() {#getMonthlyOrdinalDay--}
```
public final int getMonthlyOrdinalDay()
```


序数日を使用する場合の月次繰り返しパターンの日を取得します。

--------------------

[DayOfWeek](../../com.aspose/tasks/dayofweek) 列挙体の値のいずれかです。

**Returns:**
int - 序数日を使用する場合の月次繰り返しパターンの日。
### getMonthlyOrdinalNumber() {#getMonthlyOrdinalNumber--}
```
public final int getMonthlyOrdinalNumber()
```


月次繰り返しパターンの序数を取得します。

--------------------

[OrdinalNumber](../../com.aspose/tasks/ordinalnumber) 列挙体の値のいずれかです。

**Returns:**
int - 月次繰り返しパターンの序数。
### getMonthlyOrdinalRepetitions() {#getMonthlyOrdinalRepetitions--}
```
public final int getMonthlyOrdinalRepetitions()
```


序数日を使用する場合の月次繰り返しパターンの繰り返し回数を取得します。

**Returns:**
int - 曜日序数を使用する月次再発パターンの繰り返し回数。
### getMonthlyRepetitions() {#getMonthlyRepetitions--}
```
public final int getMonthlyRepetitions()
```


月次繰り返しパターンの繰り返し回数を取得します。

**Returns:**
int - 月次再発パターンの繰り返し回数。
### getMonthlyUseOrdinalDay() {#getMonthlyUseOrdinalDay--}
```
public final boolean getMonthlyUseOrdinalDay()
```


月次繰り返しパターンで序数日を使用するかどうかを示す値を取得します。

**Returns:**
boolean - 月次再発パターンで曜日序数を使用するかどうかを示す値。
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


繰り返しタスクの発生回数を取得します。

**Returns:**
int - 繰り返しタスクの発生回数。
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final int getRecurrencePattern()
```


繰り返しタスクの繰り返しパターンを取得します。

--------------------

`RecurrencePattern` の列挙値のいずれかです（[getRecurrencePattern()](../../com.aspose/tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose/tasks/recurringtaskinfo\#setRecurrencePattern-int-)）。

**Returns:**
int - 繰り返しタスクの再発パターン。
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


発生が開始する日付を取得します。

**Returns:**
java.util.Date - 発生開始日。
### getTask() {#getTask--}
```
public final Task getTask()
```


このインスタンスの [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) クラスの親タスクを取得します。

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class.
### getUseEndDate() {#getUseEndDate--}
```
public final boolean getUseEndDate()
```


繰り返しタスクで終了日または発生回数のいずれかを使用するかどうかを示す値を取得します。

**Returns:**
boolean - 繰り返しタスクで終了日を使用するか、発生回数を使用するかを示す値。
### getWeeklyDays() {#getWeeklyDays--}
```
public final int getWeeklyDays()
```


週次繰り返しパターンで使用される日のコレクションを取得します。

--------------------

**Returns:**
int - 週次再発パターンで使用される曜日の集合。
### getWeeklyRepetitions() {#getWeeklyRepetitions--}
```
public final int getWeeklyRepetitions()
```


週次繰り返しパターンの繰り返し回数を取得します。

**Returns:**
int - 週次再発パターンの繰り返し回数。
### getYearlyDate() {#getYearlyDate--}
```
public final Date getYearlyDate()
```


年次繰り返しパターンの日付を取得します。

**Returns:**
java.util.Date - 年次再発パターンの日付。
### getYearlyOrdinalDay() {#getYearlyOrdinalDay--}
```
public final int getYearlyOrdinalDay()
```


序数日を使用する場合の年次繰り返しパターンの曜日を取得します。

--------------------

[DayOfWeek](../../com.aspose/tasks/dayofweek) 列挙体の値のいずれかです。

**Returns:**
int - 曜日序数を使用する年次再発パターンの曜日。
### getYearlyOrdinalMonth() {#getYearlyOrdinalMonth--}
```
public final int getYearlyOrdinalMonth()
```


序数日を使用する場合の年次繰り返しパターンの月を取得します。

--------------------

[Month](../../com.aspose/tasks/month) 列挙体のいずれかの値です。

**Returns:**
int - 曜日序数を使用する年次再発パターンの月。
### getYearlyOrdinalNumber() {#getYearlyOrdinalNumber--}
```
public final int getYearlyOrdinalNumber()
```


年次繰り返しパターンの序数を取得します。

--------------------

[OrdinalNumber](../../com.aspose/tasks/ordinalnumber) 列挙体の値のいずれかです。

**Returns:**
int - 年次再発パターンの序数。
### getYearlyUseOrdinalDay() {#getYearlyUseOrdinalDay--}
```
public final boolean getYearlyUseOrdinalDay()
```


年次繰り返しパターンで序数日を使用するかどうかを示す値を取得します。

**Returns:**
boolean - 年次再発パターンで曜日序数を使用するかどうかを示す値。
### setDailyRepetitions(int value) {#setDailyRepetitions-int-}
```
public final void setDailyRepetitions(int value)
```


日次繰り返しパターンの繰り返し回数を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 日次再発パターンの繰り返し回数。 |

### setDailyUseWorkdays(boolean value) {#setDailyUseWorkdays-boolean-}
```
public final void setDailyUseWorkdays(boolean value)
```


日次繰り返しパターンで営業日を使用するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 日次再発パターンで営業日を使用するかどうかを示す値。 |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


繰り返しタスクの 1 回の発生の期間を設定します。

--------------------

`Duration` クラスのインスタンス([getDuration()](../../com.aspose/tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose/tasks/recurringtaskinfo\#setDuration-Duration-))。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | 繰り返しタスクの1回の発生期間。 |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


発生が終了する日付を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | 発生終了日。 |

### setMonthlyDay(int value) {#setMonthlyDay-int-}
```
public final void setMonthlyDay(int value)
```


月次繰り返しパターンの日数を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 月次再発パターンの日数。 |

### setMonthlyOrdinalDay(int value) {#setMonthlyOrdinalDay-int-}
```
public final void setMonthlyOrdinalDay(int value)
```


序数日を使用する場合の月次繰り返しパターンの日を設定します。

--------------------

[DayOfWeek](../../com.aspose/tasks/dayofweek) 列挙体の値のいずれかです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 曜日序数を使用する月次再発パターンの日。 |

### setMonthlyOrdinalNumber(int value) {#setMonthlyOrdinalNumber-int-}
```
public final void setMonthlyOrdinalNumber(int value)
```


月次繰り返しパターンの序数を設定します。

--------------------

[OrdinalNumber](../../com.aspose/tasks/ordinalnumber) 列挙体の値のいずれかです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 月次再発パターンの序数。 |

### setMonthlyOrdinalRepetitions(int value) {#setMonthlyOrdinalRepetitions-int-}
```
public final void setMonthlyOrdinalRepetitions(int value)
```


序数日を使用する場合の月次繰り返しパターンの繰り返し回数を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 曜日序数を使用する月次再発パターンの繰り返し回数。 |

### setMonthlyRepetitions(int value) {#setMonthlyRepetitions-int-}
```
public final void setMonthlyRepetitions(int value)
```


月次繰り返しパターンの繰り返し回数を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 月次再発パターンの繰り返し回数。 |

### setMonthlyUseOrdinalDay(boolean value) {#setMonthlyUseOrdinalDay-boolean-}
```
public final void setMonthlyUseOrdinalDay(boolean value)
```


月次繰り返しパターンで序数日を使用するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 月次の繰り返しパターンで序数日を使用するかどうかを示す値。 |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


定期タスクの発生回数を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 繰り返しタスクの発生回数。 |

### setRecurrencePattern(int value) {#setRecurrencePattern-int-}
```
public final void setRecurrencePattern(int value)
```


定期タスクの繰り返しパターンを設定します。

--------------------

`RecurrencePattern` の列挙値のいずれかです（[getRecurrencePattern()](../../com.aspose/tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose/tasks/recurringtaskinfo\#setRecurrencePattern-int-)）。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 繰り返しタスクの繰り返しパターン。 |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


発生開始日を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | 発生が開始される日付。 |

### setUseEndDate(boolean value) {#setUseEndDate-boolean-}
```
public final void setUseEndDate(boolean value)
```


定期タスクで終了日を使用するか、発生回数を使用するかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 繰り返しタスクに対して終了日を使用するか、発生回数を使用するかを示す値。 |

### setWeeklyDays(int value) {#setWeeklyDays-int-}
```
public final void setWeeklyDays(int value)
```


週次繰り返しパターンで使用される曜日のコレクションを設定します。

--------------------

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 週次の繰り返しパターンで使用される曜日のコレクション。 |

### setWeeklyRepetitions(int value) {#setWeeklyRepetitions-int-}
```
public final void setWeeklyRepetitions(int value)
```


週次繰り返しパターンの繰り返し回数を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 週次の繰り返しパターンの繰り返し回数。 |

### setYearlyDate(Date value) {#setYearlyDate-java.util.Date-}
```
public final void setYearlyDate(Date value)
```


年次繰り返しパターンの日付を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | 年次の繰り返しパターンの日付。 |

### setYearlyOrdinalDay(int value) {#setYearlyOrdinalDay-int-}
```
public final void setYearlyOrdinalDay(int value)
```


序数日を使用する場合の年次繰り返しパターンの曜日を設定します。

--------------------

[DayOfWeek](../../com.aspose/tasks/dayofweek) 列挙体の値のいずれかです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 序数日を使用する場合の年次繰り返しパターンの曜日。 |

### setYearlyOrdinalMonth(int value) {#setYearlyOrdinalMonth-int-}
```
public final void setYearlyOrdinalMonth(int value)
```


序数日を使用する場合の年次繰り返しパターンの月を設定します。

--------------------

[Month](../../com.aspose/tasks/month) 列挙体のいずれかの値です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 序数日を使用する場合の年次繰り返しパターンの月。 |

### setYearlyOrdinalNumber(int value) {#setYearlyOrdinalNumber-int-}
```
public final void setYearlyOrdinalNumber(int value)
```


年次繰り返しパターンの序数を設定します。

--------------------

[OrdinalNumber](../../com.aspose/tasks/ordinalnumber) 列挙体の値のいずれかです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 年次繰り返しパターンの序数。 |

### setYearlyUseOrdinalDay(boolean value) {#setYearlyUseOrdinalDay-boolean-}
```
public final void setYearlyUseOrdinalDay(boolean value)
```


年次繰り返しパターンで序数日を使用するかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 年次の繰り返しパターンで序数日を使用するかどうかを示す値。 |

