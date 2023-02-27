---
title: Calendar
second_title: Aspose.Tasks for .NET API リファレンス
description: プロジェクトで使用されるカレンダーを表します
type: docs
weight: 230
url: /ja/net/aspose.tasks/calendar/
---
## Calendar class

プロジェクトで使用されるカレンダーを表します。

```csharp
public class Calendar
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | このカレンダーが依存する基本カレンダーを取得または設定します。 カレンダーが基本カレンダーでない場合にのみ適用されます。 |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | CalendarExceptionCollection オブジェクトを取得します。 カレンダーに関連付けられている例外のコレクション。 |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | カレンダーが基準カレンダーかどうかを示す値を取得します。 |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | カレンダーが基準カレンダーかどうかを示す値を取得または設定します。 |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | カレンダーの名前を取得または設定します。 |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | カレンダーの一意の識別子を取得または設定します。 |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | このカレンダーの WeekDaysCollection を取得します。 カレンダーを定義する曜日のコレクション。 |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | WorkWeekCollections オブジェクトを取得します。 カレンダーに関連付けられた稼働週のコレクション。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | 指定されたカレンダーを 24 時間カレンダーにします。 24 時間カレンダーは、すべての曜日が 24 時間体制で稼働するカレンダーです。 |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | 指定されたカレンダーを夜勤カレンダーにします。 |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | デフォルトの標準カレンダーを作成します。 |
| [Delete](../../aspose.tasks/calendar/delete/)() | プロジェクトからカレンダーを削除します。 |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | カレンダーに従って、指定された作業時間が経過する日付を計算します。 |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | カレンダーに従って、指定された作業時間が経過する日付を計算します。 |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | クラスのインスタンスのハッシュ コードを返します。 |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | 日付から翌営業日開始を計算します。 |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | 指定した日付から前の稼働日の終了日を計算します。 |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | 指定された FinishDate と Duration に基づいて StartDate を返します。 |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | 指定された FinishDate と Duration に基づいて StartDate を返します。 |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | タスクの開始日、分割部分、期間からタスクの終了日時を計算します。 |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | 日付の労働時間を返します。 |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | 指定された日付の稼働時間を返します。 |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | 戻り値[`WorkingTimeCollection`](../workingtimecollection/)指定された日付の稼働時間. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | その日が稼働日かどうかを判別します。 |

### 備考

カレンダーは、標準の稼働時間と非稼働時間を定義するために使用されます。 プロジェクトには 1 つの基本カレンダーが必要です。タスクとリソースは、基本カレンダーに基づく独自の非基本カレンダーを 持つことができます.

### 例

シンプルなカレンダーを一から作る方法.

```csharp
[C#]
// 空のカレンダーを作成
Calendar calendar = new Calendar("New calendar");
// デフォルトの稼働日を追加します (9:00 から 17:00 までの 8 稼働時間)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// 新しい新しい営業日を作成します
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// 勤務時間を設定します。 DateTime の時間部分のみが重要です
    WorkingTime wt1 = new WorkingTime();
    wt1.FromTime = new DateTime(1, 1, 1, 6, 0, 0, 0);
    wt1.ToTime = new DateTime(1, 1, 1, 12, 0, 0, 0);
    WorkingTime wt2 = new WorkingTime();
    wt2.FromTime = new DateTime(1, 1, 1, 14, 0, 0, 0);
    wt2.ToTime = new DateTime(1, 1, 1, 18, 0, 0, 0);
    myWeekDay.WorkingTimes.Add(wt1);
    myWeekDay.WorkingTimes.Add(wt2);
    myWeekDay.DayWorking = true;
calendar.Days.Add(myWeekDay);
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
// 週末を追加
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
'空のカレンダーを作成する
Dim calendar As Calendar =  New Calendar("New calendar")
'デフォルトの稼働日を追加 (9:00 から 17:00 までの 8 稼働時間)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
'新しい新しい営業日を作成する
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
'作業時間を設定します。 DateTime の時間部分のみが重要です
    Dim wt1 As WorkingTime =  New WorkingTime()
    wt1.FromTime = New DateTime(1, 1, 1, 6, 0, 0, 0)
    wt1.ToTime = New DateTime(1, 1, 1, 12, 0, 0, 0)
    Dim wt2 As WorkingTime =  New WorkingTime()
    wt2.FromTime = New DateTime(1, 1, 1, 14, 0, 0, 0)
    wt2.ToTime = New DateTime(1, 1, 1, 18, 0, 0, 0)
    myWeekDay.WorkingTimes.Add(wt1)
    myWeekDay.WorkingTimes.Add(wt2)
    myWeekDay.DayWorking = True
calendar.Days.Add(myWeekDay)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday))
'週末を追加
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

### 関連項目

* 名前空間 [Aspose.Tasks](../../aspose.tasks/)
* 組み立て [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
