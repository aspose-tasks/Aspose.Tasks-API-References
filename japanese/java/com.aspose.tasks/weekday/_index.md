---
title: "WeekDay"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "カレンダーで通常の曜日または例外日を定義する平日を表します。"
type: docs
weight: 352
url: /ja/java/com.aspose.tasks/weekday/
---

**Inheritance:**
java.lang.Object
```
public class WeekDay
```

カレンダーで通常の曜日または例外日を定義する平日を表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [WeekDay(int dayType)](#WeekDay-int-) | 指定された日タイプで[WeekDay](../../com.aspose.tasks/weekday)クラスの新しいインスタンスを初期化します。 |
| [WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes)](#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--) | 指定された日タイプと作業時間期間のリストで[WeekDay](../../com.aspose.tasks/weekday)クラスの新しいインスタンスを初期化します。 |
| [WeekDay(int dayType, WorkingTime[] workingTimes)](#WeekDay-int-com.aspose.tasks.WorkingTime...-) | 指定された日タイプと作業時間期間で[WeekDay](../../com.aspose.tasks/weekday)クラスの新しいインスタンスを初期化します。 |
| [WeekDay()](#WeekDay--) | [WeekDay](../../com.aspose.tasks/weekday)クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [castToDayType(int dw)](#castToDayType-int-) | .Net の[DayOfWeek](../../com.aspose.tasks/dayofweek)を`DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-))にキャストします。 |
| [createDefaultWorkingDay(int dayType)](#createDefaultWorkingDay-int-) | デフォルトの作業日を作成します。 |
| [deepClone()](#deepClone--) | 週日のディープコピーを返します。 |
| [equals(Object obj)](#equals-java.lang.Object-) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [getDayType()](#getDayType--) | 日のタイプを取得します。 |
| [getDayWorking()](#getDayWorking--) | 指定された日付または日タイプが作業日かどうかを示す値を取得します。 |
| [getFromDate()](#getFromDate--) | 例外時間の開始時刻を取得します。 |
| [getToDate()](#getToDate--) | 例外時間の終了時刻を取得します。 |
| [getWorkingTime()](#getWorkingTime--) | 週日の作業時間を返します。 |
| [getWorkingTimes()](#getWorkingTimes--) | この WeekDay インスタンスの WorkingTimeCollection を取得します。 |
| [hashCode()](#hashCode--) | [WeekDay](../../com.aspose.tasks/weekday) クラスのインスタンスに対するハッシュコード値を返します。 |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | 指定された日付または曜日タイプが稼働しているかどうかを示す値を設定します。 |
| [setDefaultWorkingTime(WeekDay day)](#setDefaultWorkingTime-com.aspose.tasks.WeekDay-) | 指定された曜日のデフォルトの時間帯を設定します。 |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | 例外時間の開始時刻を設定します。 |
| [setToDate(Date value)](#setToDate-java.util.Date-) | 例外時間の終了時刻を設定します。 |
### WeekDay(int dayType) {#WeekDay-int-}
```
public WeekDay(int dayType)
```


指定された日タイプで[WeekDay](../../com.aspose.tasks/weekday)クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dayType | int | 指定された day type。 |

### WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes) {#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--}
```
public WeekDay(int dayType, List<WorkingTime> workingTimes)
```


指定された日タイプと作業時間期間のリストで[WeekDay](../../com.aspose.tasks/weekday)クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dayType | int | 指定された day type。 |
| workingTimes | java.util.List&lt;com.aspose.tasks.WorkingTime&gt; | 作業時間帯のリスト。 |

### WeekDay(int dayType, WorkingTime[] workingTimes) {#WeekDay-int-com.aspose.tasks.WorkingTime...-}
```
public WeekDay(int dayType, WorkingTime[] workingTimes)
```


指定された日タイプと作業時間期間で[WeekDay](../../com.aspose.tasks/weekday)クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dayType | int | 指定された day type。 |
| workingTimes | [WorkingTime\[\]](../../com.aspose.tasks/workingtime) | 作業時間帯の配列。 |

### WeekDay() {#WeekDay--}
```
public WeekDay()
```


[WeekDay](../../com.aspose.tasks/weekday)クラスの新しいインスタンスを初期化します。

### castToDayType(int dw) {#castToDayType-int-}
```
public static int castToDayType(int dw)
```


.Net の[DayOfWeek](../../com.aspose.tasks/dayofweek)を`DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-))にキャストします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dw | int | キャスト元の曜日。 |

**Returns:**
int - キャストされた曜日タイプ。
### createDefaultWorkingDay(int dayType) {#createDefaultWorkingDay-int-}
```
public static WeekDay createDefaultWorkingDay(int dayType)
```


デフォルトの作業日を作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dayType | int | デフォルトの稼働日を作成する元となる曜日タイプ。 |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - A default working day with working times 8-12 and 13-17.
### deepClone() {#deepClone--}
```
public final WeekDay deepClone()
```


週日のディープコピーを返します。

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - Returns the deep copy of the week day.
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
boolean - 指定されたオブジェクトがこのインスタンスと同じ FromDate、ToDate の値および WorkingTimes を持つ WeekDay である場合は **True**、それ以外の場合は **false**。
### getDayType() {#getDayType--}
```
public final int getDayType()
```


日のタイプを取得します。

**Returns:**
int - 曜日のタイプ。
### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


指定された日付または日タイプが作業日かどうかを示す値を取得します。

**Returns:**
boolean - 指定された日付または曜日タイプが稼働しているかどうかを示す値。
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


例外時間の開始時刻を取得します。

**Returns:**
java.util.Date - 例外時間の開始時刻。
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


例外時間の終了時刻を取得します。

**Returns:**
java.util.Date - 例外時間の終了時刻。
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


週日の作業時間を返します。

**Returns:**
double - 作業時間。
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


この WeekDay インスタンスの WorkingTimeCollection を取得します。曜日での作業時間を定義する作業時間のコレクションです。

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - WorkingTimeCollection for this WeekDay instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```


[WeekDay](../../com.aspose.tasks/weekday) クラスのインスタンスに対するハッシュコード値を返します。

**Returns:**
int - このオブジェクトのハッシュコード値を返します。
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


指定された日付または曜日タイプが稼働しているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 指定された日付または曜日タイプが稼働しているかどうかを示す値。 |

### setDefaultWorkingTime(WeekDay day) {#setDefaultWorkingTime-com.aspose.tasks.WeekDay-}
```
public static void setDefaultWorkingTime(WeekDay day)
```


指定された曜日のデフォルトの時間帯を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| day | [WeekDay](../../com.aspose.tasks/weekday) | デフォルトの稼働日を設定する曜日。 |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


例外時間の開始時刻を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | 例外時間の開始。 |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


例外時間の終了時刻を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | 例外時間の終了。 |

