---
title: "CalendarException"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "カレンダー内の例外的な時間期間を表します。"
type: docs
weight: 43
url: /ja/java/com.aspose.tasks/calendarexception/
---

**Inheritance:**
java.lang.Object
```
public final class CalendarException
```

カレンダー内の例外的な時間期間を表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [CalendarException()](#CalendarException--) | [CalendarException](../../com.aspose.tasks/calendarexception) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [checkException(Date dt)](#checkException-java.util.Date-) | 指定された java.util.Date 構造体のインスタンスが例外日である場合、true を返します。 |
| [delete()](#delete--) | 親カレンダーの CalendarExceptionCollection オブジェクトから例外インスタンスを削除します。 |
| [getDayWorking()](#getDayWorking--) | 指定された日付または日タイプが作業日かどうかを示す値を取得します。 |
| [getDaysOfWeek()](#getDaysOfWeek--) | このオブジェクトの DayTypeCollection を取得します。 |
| [getEnteredByOccurrences()](#getEnteredByOccurrences--) | 繰り返し範囲が発生回数の入力によって定義されているかどうかを示す値を取得します。 |
| [getExceptionDates()](#getExceptionDates--) | カレンダー例外が適用される日付を返します。 |
| [getFromDate()](#getFromDate--) | 例外時間の開始時刻を取得します。 |
| [getMonth()](#getMonth--) | 例外の繰り返しが予定されている月を取得します。 |
| [getMonthDay()](#getMonthDay--) | 例外の繰り返しが予定されている月の日を取得します。 |
| [getMonthItem()](#getMonthItem--) | 例外の繰り返しが予定されている月項目を取得します。 |
| [getMonthPosition()](#getMonthPosition--) | 月内の月項目の位置を取得します。 |
| [getName()](#getName--) | 例外の名前を取得します。 |
| [getOccurrences()](#getOccurrences--) | カレンダー例外が有効な発生回数を取得します。 |
| [getParentCalendar()](#getParentCalendar--) | このオブジェクトの親カレンダーを取得します。 |
| [getPeriod()](#getPeriod--) | 例外の繰り返し期間を取得します。 |
| [getToDate()](#getToDate--) | 例外時間の終了時刻を取得します。 |
| [getType()](#getType--) | 例外のタイプを取得します。 |
| [getWorkingTime()](#getWorkingTime--) | カレンダー例外の作業時間を返します。 |
| [getWorkingTimes()](#getWorkingTimes--) | WorkingTimeCollection オブジェクトを取得します。 |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | 指定された日付または曜日タイプが稼働しているかどうかを示す値を設定します。 |
| [setEnteredByOccurrences(boolean value)](#setEnteredByOccurrences-boolean-) | 繰り返し範囲が発生回数の入力によって定義されているかどうかを示す値を設定します。 |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | 例外時間の開始時刻を設定します。 |
| [setMonth(int value)](#setMonth-int-) | 例外の繰り返しが予定されている月を設定します。 |
| [setMonthDay(int value)](#setMonthDay-int-) | 例外の繰り返しが予定されている月の日を設定します。 |
| [setMonthItem(int value)](#setMonthItem-int-) | 例外の繰り返しが予定されている月項目を設定します。 |
| [setMonthPosition(int value)](#setMonthPosition-int-) | 月内の月項目の位置を設定します。 |
| [setName(String value)](#setName-java.lang.String-) | 例外の名前を設定します。 |
| [setOccurrences(int value)](#setOccurrences-int-) | カレンダー例外が有効な発生回数を設定します。 |
| [setPeriod(int value)](#setPeriod-int-) | 例外の繰り返し期間を設定します。 |
| [setToDate(Date value)](#setToDate-java.util.Date-) | 例外時間の終了時刻を設定します。 |
| [setType(int value)](#setType-int-) | 例外タイプを設定します。 |
| [setWorkingTimes(WorkingTimeCollection value)](#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-) | WorkingTimeCollection オブジェクトを設定します。 |
### CalendarException() {#CalendarException--}
```
public CalendarException()
```


[CalendarException](../../com.aspose.tasks/calendarexception) クラスの新しいインスタンスを初期化します。

### checkException(Date dt) {#checkException-java.util.Date-}
```
public final boolean checkException(Date dt)
```


指定された java.util.Date 構造体のインスタンスが例外日である場合、true を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dt | java.util.Date | 指定された java.util.Date 構造体のインスタンス。 |

**Returns:**
boolean - java.util.Date の値が例外日である場合は true を返し、そうでない場合は false を返します。
### delete() {#delete--}
```
public final void delete()
```


親カレンダーの CalendarExceptionCollection オブジェクトから例外インスタンスを削除します。

### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


指定された日付または日タイプが作業日かどうかを示す値を取得します。

**Returns:**
boolean - 指定された日付または曜日タイプが稼働しているかどうかを示す値。
### getDaysOfWeek() {#getDaysOfWeek--}
```
public final DayTypeCollection getDaysOfWeek()
```


このオブジェクトの DayTypeCollection を取得します。例外が有効な曜日。

**Returns:**
[DayTypeCollection](../../com.aspose.tasks/daytypecollection) - the DayTypeCollection for this object.
### getEnteredByOccurrences() {#getEnteredByOccurrences--}
```
public final boolean getEnteredByOccurrences()
```


繰り返し範囲が発生回数の入力によって定義されているかを示す値を取得します。False は、繰り返し範囲が終了日を入力して定義されていることを示します。

**Returns:**
boolean - 繰り返し範囲が発生回数の入力によって定義されているかを示す値。
### getExceptionDates() {#getExceptionDates--}
```
public final Iterable<Date> getExceptionDates()
```


カレンダー例外が適用される日付を返します。

**Returns:**
java.lang.Iterable&lt;java.util.Date&gt; - カレンダー例外が適用される日付。
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


例外時間の開始時刻を取得します。

**Returns:**
java.util.Date - 例外時間の開始。
### getMonth() {#getMonth--}
```
public final int getMonth()
```


例外の繰り返しが予定されている月を取得します。

**Returns:**
int - 例外の繰り返しが予定されている月。
### getMonthDay() {#getMonthDay--}
```
public final int getMonthDay()
```


例外の繰り返しが予定されている月の日を取得します。

**Returns:**
int - 例外の繰り返しが予定されている月の日。
### getMonthItem() {#getMonthItem--}
```
public final int getMonthItem()
```


例外の繰り返しが予定されている月項目を取得します。

**Returns:**
int - 例外の繰り返しが予定されている月項目。
### getMonthPosition() {#getMonthPosition--}
```
public final int getMonthPosition()
```


月内の月項目の位置を取得します。

**Returns:**
int - 月内の月項目の位置。
### getName() {#getName--}
```
public final String getName()
```


例外の名前を取得します。

**Returns:**
java.lang.String - 例外の名前。
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


カレンダー例外が有効な発生回数を取得します。

**Returns:**
int - カレンダー例外が有効な発生回数。
### getParentCalendar() {#getParentCalendar--}
```
public final Calendar getParentCalendar()
```


このオブジェクトの親カレンダーを取得します。

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - the parent calendar for this object.
### getPeriod() {#getPeriod--}
```
public final int getPeriod()
```


例外の繰り返し期間を取得します。

**Returns:**
int - 例外の繰り返し期間。
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


例外時間の終了時刻を取得します。

**Returns:**
java.util.Date - 例外時間の終了。
### getType() {#getType--}
```
public final int getType()
```


例外のタイプを取得します。

**Returns:**
int - 例外タイプ。
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


カレンダー例外の作業時間を返します。

**Returns:**
double - このカレンダー例外の作業時間を返します。
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


WorkingTimeCollection オブジェクトを取得します。平日に作業した時間を定義する作業時間のコレクションです。

--------------------

少なくとも1つの作業時間が必要で、5つを超えてはいけません。

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - the WorkingTimeCollection object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


指定された日付または曜日タイプが稼働しているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 指定された日付または曜日タイプが稼働しているかどうかを示す値。 |

### setEnteredByOccurrences(boolean value) {#setEnteredByOccurrences-boolean-}
```
public final void setEnteredByOccurrences(boolean value)
```


繰り返し範囲が発生回数の入力によって定義されているかを示す値を設定します。False は、繰り返し範囲が終了日を入力して定義されていることを示します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 繰り返し範囲が発生回数の入力によって定義されているかを示す値。 |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


例外時間の開始時刻を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | 例外時間の開始。 |

### setMonth(int value) {#setMonth-int-}
```
public final void setMonth(int value)
```


例外の繰り返しが予定されている月を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 例外の繰り返しが予定されている月。 |

### setMonthDay(int value) {#setMonthDay-int-}
```
public final void setMonthDay(int value)
```


例外の繰り返しが予定されている月の日を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 例外の繰り返しが予定されている月の日。 |

### setMonthItem(int value) {#setMonthItem-int-}
```
public final void setMonthItem(int value)
```


例外の繰り返しが予定されている月項目を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 例外の繰り返しが予定されている月の項目。 |

### setMonthPosition(int value) {#setMonthPosition-int-}
```
public final void setMonthPosition(int value)
```


月内の月項目の位置を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 月内の月項目の位置。 |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


例外の名前を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 例外の名前。 |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


カレンダー例外が有効な発生回数を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | カレンダー例外が有効な発生回数。 |

### setPeriod(int value) {#setPeriod-int-}
```
public final void setPeriod(int value)
```


例外の繰り返し期間を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 例外の繰り返し期間。 |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


例外時間の終了時刻を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | 例外時間の終了。 |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


例外タイプを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 例外の種類。 |

### setWorkingTimes(WorkingTimeCollection value) {#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-}
```
public final void setWorkingTimes(WorkingTimeCollection value)
```


WorkingTimeCollection オブジェクトを設定します。平日に作業した時間を定義する作業時間のコレクション。

--------------------

少なくとも1つの作業時間が必要で、5つを超えてはいけません。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) | WorkingTimeCollection オブジェクト。 |

