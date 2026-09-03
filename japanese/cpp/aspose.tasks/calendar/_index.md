---
title: "Aspose::Tasks::Calendar クラス"
linktitle: "カレンダー"
articleTitle: "カレンダー"
second_title: "Aspose.Tasks for C++"
description: "プロジェクトで使用されるカレンダーを表します。"
type: docs
weight: 10
url: /ja/cpp/aspose.tasks/calendar/
---

## Calendar class

**Inherits:** Aspose::Tasks::ICalendar

プロジェクトで使用されるカレンダーを表します。

最初からシンプルなカレンダーを作成する方法。

```cpp
[C#]
// 空のカレンダーを作成する
Calendar calendar = new Calendar("New calendar");
// デフォルトの作業日を追加します（9:00 から 17:00 の 8 時間）。
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// 新しい作業日を作成する
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// 作業時間を設定します。DateTime の時間部分だけが重要です。
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
// 週末を追加します
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```cpp
[VB]
' create empty calendar
Dim calendar As Calendar =  New Calendar("New calendar")
' adds default working days (8 working hours from 9:00 to 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' create new new working day
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Sets working time. Only time part of DateTime is important
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
' adds weekend
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

カレンダーは標準の作業時間と非作業時間を定義するために使用されます。プロジェクトは 1 つのベース カレンダーを持つ必要があります。タスクやリソースは、ベース カレンダーに基づく独自の非ベース カレンダーを持つことができます。

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Delete](./delete/) | プロジェクトからカレンダーを削除します。 |
| [Equals](./equals/) | このインスタンスが指定されたオブジェクトと等しいかどうかを示す値を返します。 |
| [get_BaseCalendar](./get_basecalendar/) | このカレンダーが依存する基底カレンダーを取得します。カレンダーが基底カレンダーでない場合にのみ適用されます。 |
| [get_Exceptions](./get_exceptions/) | CalendarExceptionCollection オブジェクトを取得します。カレンダーに関連付けられた例外のコレクションです。 |
| [get_Guid](./get_guid/) | カレンダーの Guid を取得します。 |
| [get_IsBaseCalendar](./get_isbasecalendar/) | カレンダーが基底カレンダーかどうかを示す値を取得します。 |
| [get_IsBaselineCalendar](./get_isbaselinecalendar/) | カレンダーがベースラインカレンダーかどうかを示す値を取得します。 |
| [get_Name](./get_name/) | カレンダーの名前を取得します。 |
| [get_Uid](./get_uid/) | カレンダーの一意識別子を取得します。 |
| [get_WeekDays](./get_weekdays/) | このカレンダーの WeekDaysCollection を取得します。カレンダーを定義する曜日のコレクションです。 |
| [get_WorkWeeks](./get_workweeks/) | WorkWeekCollections オブジェクトを取得します。カレンダーに関連付けられた作業週のコレクションです。 |
| [GetFinishDateByStartAndWork (2 overloads)](./getfinishdatebystartandwork/) | カレンダーに従って、指定された作業時間が経過する日時を計算します。 |
| [GetHashCode](./gethashcode/) | クラスのインスタンスのハッシュコードを返します。 |
| [GetIntersectionCalendar](./getintersectioncalendar/) | 2 つのカレンダーの作業スケジュールの交差点で計算を実行できる ICalendar インスタンスを取得します。 |
| [GetNextWorkingDayStart](./getnextworkingdaystart/) | 指定された日付の次の稼働日の開始時刻を計算します。 |
| [GetPreviousWorkingDayEnd](./getpreviousworkingdayend/) | 指定された日付から前の稼働日の終了時刻を計算します。 |
| [GetStartDateFromFinishAndDuration (2 overloads)](./getstartdatefromfinishandduration/) | 指定された終了日と期間に基づいて開始日を返します。 |
| [GetTaskFinishDateFromDuration](./gettaskfinishdatefromduration/) | タスクの開始日、分割部分、および作業期間からタスクの終了日と時刻を計算します。 |
| [GetWorkingHours (2 overloads)](./getworkinghours/) | 指定された日付の作業時間数を返します。 |
| [GetWorkingHoursTimeSpan](./getworkinghourstimespan/) | 指定された日付間の作業時間数を返します。 |
| [GetWorkingTimes](./getworkingtimes/) | 指定された日付の作業時間の WorkingTimeCollection を返します。 |
| [GetWorkStart](./getworkstart/) | 指定された日付と時刻から始まる次の作業開始時刻を計算します。 |
| [IsDayWorking](./isdayworking/) | 指定された日がカレンダーに基づく稼働日かどうかを判定します。 |
| [IsEmpty](./isempty/) | カレンダーに作業時間が定義されていないかどうかを返します。 |
| [Make24HourCalendar](./make24hourcalendar/) | 指定されたカレンダーを 24Hour Calendar にします。24Hours Calendar は、週のすべての日が 24 時間体制で稼働するカレンダーです。 |
| [MakeNightShiftCalendar](./makenightshiftcalendar/) | 指定されたカレンダーを Night Shift Calendar にします。 |
| [MakeStandardCalendar](./makestandardcalendar/) | デフォルトの標準カレンダーを作成します。 |
| [set_BaseCalendar](./set_basecalendar/) | このカレンダーが依存する基底カレンダーを設定します。カレンダーが基底カレンダーでない場合にのみ適用されます。 |
| [set_IsBaselineCalendar](./set_isbaselinecalendar/) | カレンダーがベースラインカレンダーかどうかを示す値を設定します。 |
| [set_Name](./set_name/) | カレンダーの名前を設定します。 |
| [set_Uid](./set_uid/) | カレンダーの一意識別子を設定します。 |

