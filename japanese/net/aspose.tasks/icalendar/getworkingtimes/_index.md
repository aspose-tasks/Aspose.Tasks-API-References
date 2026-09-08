---
title: "ICalendar.GetWorkingTimes"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "ICalendar method. 指定された日の作業時間の WorkingTimeCollection を返します"
type: docs
weight: 80
url: /ja/net/aspose.tasks/icalendar/getworkingtimes/
---
## ICalendar.GetWorkingTimes method

指定された日の作業時間の [`WorkingTimeCollection`](../../workingtimecollection/) を返します。

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dt | DateTime | 作業時間を取得する日付。 |

### 戻り値

[`WorkingTime`](../../workingtime/) インスタンスのコレクション。

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

* class [WorkingTimeCollection](../../workingtimecollection/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


