---
title: "Calendar.GetIntersectionCalendar"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Calendar メソッド。2 つのカレンダーの作業スケジュールの交差点で計算を実行できる ICalendar インスタンスを取得します"
type: docs
weight: 280
url: /ja/net/aspose.tasks/calendar/getintersectioncalendar/
---
## Calendar.GetIntersectionCalendar method

2 つのカレンダーの作業スケジュールの交差点で計算を実行できる [`ICalendar`](../../icalendar/) インスタンスを取得します。

```csharp
public static ICalendar GetIntersectionCalendar(Calendar calendar1, Calendar calendar2)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| calendar1 | Calendar | 最初のカレンダーです。 |
| calendar2 | Calendar | 2 番目のカレンダーです。 |

### 戻り値

ICalendar インターフェイスの実装です。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | 引数のいずれかが null の場合です。 |

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

* interface [ICalendar](../../icalendar/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


