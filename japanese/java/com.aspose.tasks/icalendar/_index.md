---
title: "ICalendar"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "日付と期間のさまざまな計算に使用できるカレンダー抽象化を表します。"
type: docs
weight: 376
url: /ja/java/com.aspose.tasks/icalendar/
---
```
public interface ICalendar
```

日付と期間のさまざまな計算に使用できるカレンダー抽象化を表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getFinishDateByStartAndWork(Date start, Duration work)](#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-) | カレンダーに従って、指定された作業時間が経過する日時を計算します。 |
| [getFinishDateByStartAndWork(Date start, double work)](#getFinishDateByStartAndWork-java.util.Date-double-) | カレンダーに従って、指定された作業時間が経過する日時を計算します。 |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | 指定された日付の次の稼働日の開始時刻を計算します。 |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | 指定された日付から前の稼働日の終了時刻を計算します。 |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | 指定された完了日と期間に基づいて開始日を返します。 |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | 指定された完了日と期間に基づいて開始日を返します。 |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | タスクの開始日、分割部分、作業期間から完了日時を計算します。 |
| [getWorkStart(Date date)](#getWorkStart-java.util.Date-) | 指定された日時から次の稼働時間の開始時刻を計算します。 |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | 指定された日における稼働時間の量を返します。 |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | WorkUnit を返します - 指定された日時間隔の稼働時間の開始、完了、期間。 |
| [getWorkingHoursTimeSpan(Date start, Date finish)](#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-) | 指定された日付間の稼働時間の量を返します。 |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | 指定された日の稼働時間の [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) を返します。 |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | カレンダーに従って、指定された日が稼働日かどうかを判定します。 |
| [isEmpty()](#isEmpty--) | カレンダーに稼働時間が定義されていないかどうかを返します。 |
### getFinishDateByStartAndWork(Date start, Duration work) {#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getFinishDateByStartAndWork(Date start, Duration work)
```


カレンダーに従って、指定された作業時間が経過する日時を計算します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 開始 | java.util.Date | 開始日。 |
| work | [Duration](../../com.aspose.tasks/duration) | 作業期間。 |

**Returns:**
java.util.Date - 完了日。
### getFinishDateByStartAndWork(Date start, double work) {#getFinishDateByStartAndWork-java.util.Date-double-}
```
public abstract Date getFinishDateByStartAndWork(Date start, double work)
```


カレンダーに従って、指定された作業時間が経過する日時を計算します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 開始 | java.util.Date | 開始日。 |
| 作業 | double | 作業期間。 |

**Returns:**
java.util.Date - 完了日。
### getNextWorkingDayStart(Date date) {#getNextWorkingDayStart-java.util.Date-}
```
public abstract Date getNextWorkingDayStart(Date date)
```


指定された日付の次の稼働日の開始時刻を計算します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 日付 | java.util.Date | 次の営業日の開始を取得する日付。 |

**Returns:**
java.util.Date - 次の営業日の開始 System.DateTime。
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public abstract Date getPreviousWorkingDayEnd(Date date)
```


指定された日付から前の稼働日の終了時刻を計算します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 日付 | java.util.Date | 前の営業日の終了を計算する日付。 |

**Returns:**
java.util.Date - 前の営業日の終了
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
```


指定された完了日と期間に基づいて開始日を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 終了 | java.util.Date | 指定された終了日。 |
| duration | [Duration](../../com.aspose.tasks/duration) | 指定された期間。 |

**Returns:**
java.util.Date - 計算された開始日。
### getStartDateFromFinishAndDuration(Date finish, double duration) {#getStartDateFromFinishAndDuration-java.util.Date-double-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, double duration)
```


指定された完了日と期間に基づいて開始日を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 終了 | java.util.Date | 指定された終了日。 |
| 期間 | double | 指定された期間。 |

**Returns:**
java.util.Date - 計算された開始日。
### getTaskFinishDateFromDuration(Task task, double duration) {#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-}
```
public abstract Date getTaskFinishDateFromDuration(Task task, double duration)
```


タスクの開始日、分割部分、作業期間から完了日時を計算します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 終了日を計算するタスク。 |
|  | 期間 | double | 計算する期間。 |

タスクがサマリーであるか、null、または開始日が設定されていない場合は DateTime.MinValue を返します。 |

**Returns:**
java.util.Date - 指定された開始日と期間に対するタスクの終了日。
### getWorkStart(Date date) {#getWorkStart-java.util.Date-}
```
public abstract Date getWorkStart(Date date)
```


指定された日時から次の稼働時間の開始時刻を計算します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 日付 | java.util.Date | 日付と時刻。 |

**Returns:**
java.util.Date - 最も近い営業時間の開始。
### getWorkingHours(Date dt) {#getWorkingHours-java.util.Date-}
```
public abstract double getWorkingHours(Date dt)
```


指定された日における稼働時間の量を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dt | java.util.Date | 作業時間を取得する日付。 |

**Returns:**
double - 指定された日付の作業時間。
### getWorkingHours(Date start, Date finish) {#getWorkingHours-java.util.Date-java.util.Date-}
```
public abstract WorkUnit getWorkingHours(Date start, Date finish)
```


WorkUnit を返します - 指定された日時間隔の稼働時間の開始、完了、期間。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 開始 | java.util.Date | 間隔の開始日。 |
| 終了 | java.util.Date | 間隔の終了日。 |

**Returns:**
[WorkUnit](../../com.aspose.tasks/workunit) - Instance of [WorkUnit](../../com.aspose.tasks/workunit) class containing Start, Finish and Duration of working hours.
### getWorkingHoursTimeSpan(Date start, Date finish) {#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-}
```
public abstract double getWorkingHoursTimeSpan(Date start, Date finish)
```


指定された日付間の稼働時間の量を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 開始 | java.util.Date | 間隔の開始日。 |
| 終了 | java.util.Date | 間隔の終了日。 |

**Returns:**
double - カレンダーインスタンスに基づく作業時間の量。
### getWorkingTimes(Date dt) {#getWorkingTimes-java.util.Date-}
```
public abstract WorkingTimeCollection getWorkingTimes(Date dt)
```


指定された日の稼働時間の [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dt | java.util.Date | 作業時間を取得する日付。 |

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - Collection of [WorkingTime](../../com.aspose.tasks/workingtime) instances.
### isDayWorking(Date dt) {#isDayWorking-java.util.Date-}
```
public abstract boolean isDayWorking(Date dt)
```


カレンダーに従って、指定された日が稼働日かどうかを判定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dt | java.util.Date | その日が営業日かどうかを確認する日付。 |

**Returns:**
boolean - その日が営業日であれば true。
### isEmpty() {#isEmpty--}
```
public abstract boolean isEmpty()
```


カレンダーに稼働時間が定義されていないかどうかを返します。

**Returns:**
boolean - カレンダーに作業時間が定義されていない場合は true です。
