---
title: "インターフェイス ICalendar"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Aspose.Tasks.ICalendar インターフェイス。日付や期間のさまざまな計算に使用できるカレンダー抽象を表します。"
type: docs
weight: 840
url: /ja/net/aspose.tasks/icalendar/
---
## ICalendar interface

日付や期間のさまざまな計算に使用できるカレンダー抽象を表します。

```csharp
public interface ICalendar
```

## メソッド

| 名前 | 説明 |
| --- | --- |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | カレンダーに従って、指定された作業時間が経過する日時を計算します。 |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | カレンダーに従って、指定された作業時間が経過する日時を計算します。 |
| [GetNextWorkingDayStart](../../aspose.tasks/icalendar/getnextworkingdaystart/)(DateTime) | 指定された日付の次の稼働日の開始時刻を計算します。 |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/icalendar/getpreviousworkingdayend/)(DateTime) | 指定された日付から前の稼働日の終了時刻を計算します。 |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | 指定された終了日と期間に基づいて開始日を返します。 |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | 指定された終了日と期間に基づいて開始日を返します。 |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/icalendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | タスクの開始日、分割部分、作業期間からタスクの終了日時を計算します。 |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours_1)(DateTime) | 指定された日付の作業時間量を返します。 |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | 指定された日時間隔の作業時間の開始、終了、期間を示す WorkUnit を返します。 |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/icalendar/getworkinghourstimespan/)(DateTime, DateTime) | 指定された日付間の作業時間量を返します。 |
| [GetWorkingTimes](../../aspose.tasks/icalendar/getworkingtimes/)(DateTime) | 指定された日付の作業時間の [`WorkingTimeCollection`](../workingtimecollection/) を返します。 |
| [GetWorkStart](../../aspose.tasks/icalendar/getworkstart/)(DateTime) | 指定された日時から始まる次の作業時間開始時刻を計算します。 |
| [IsDayWorking](../../aspose.tasks/icalendar/isdayworking/)(DateTime) | 指定された日がカレンダー上で稼働日かどうかを判定します。 |
| [IsEmpty](../../aspose.tasks/icalendar/isempty/)() | カレンダーに作業時間が定義されていないかどうかを返します。 |

## 例

Calendar.GetIntersectionCalendar() メソッドの使用方法を示し、割り当てのカレンダーで計算を実行します。

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

foreach (var ra in project.ResourceAssignments)
{
    if (ra.Resource == null)
    {
        continue;
    }

    ICalendar assignmentCalendar;

    Calendar taskCalendar = ra.Task.Calendar != null && !ra.Task.Duration.IsEstimated ? ra.Task.Calendar : null;
    Calendar resourceCalendar = ra.Resource.Calendar != null && !ra.Task.IgnoreResourceCalendar
        ? ra.Resource.Calendar
        : null;

    if (taskCalendar != null && resourceCalendar != null && !ReferenceEquals(taskCalendar, resourceCalendar))
    {
        assignmentCalendar = Calendar.GetIntersectionCalendar(taskCalendar, resourceCalendar);
    }
    else
    {
        assignmentCalendar = taskCalendar ?? resourceCalendar;
    }

    if (assignmentCalendar == null)
    {
        assignmentCalendar = project.Calendar;
    }

    var workingHours = assignmentCalendar.GetWorkingHours(ra.Start, ra.Finish);

    Console.WriteLine("Working hours for assignment '{0}' : {1}", ra, workingHours);

    var date = new DateTime(2025, 4, 7);
    Console.WriteLine("Working times for date '{0}':", date);

    foreach (var wt in assignmentCalendar.GetWorkingTimes(date))
    {
        Console.WriteLine("{0} - {1}", wt.From.TimeOfDay, wt.To.TimeOfDay);
    }
}
```

### 関連項目

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


