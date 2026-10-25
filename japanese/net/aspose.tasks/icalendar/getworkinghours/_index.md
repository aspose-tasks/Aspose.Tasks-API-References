---
title: "ICalendar.GetWorkingHours"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "ICalendar メソッド。指定された日時間隔の作業時間に関する WorkUnit、Start、Finish、Duration を返します。"
type: docs
weight: 60
url: /ja/net/aspose.tasks/icalendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

指定された日時間隔の作業時間の開始、終了、期間を示す WorkUnit を返します。

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| start | DateTime | 期間の開始日。 |
| finish | DateTime | 期間の終了日。 |

### 戻り値

[`WorkUnit`](../../workunit/) クラスのインスタンスで、作業時間の Start、Finish、Duration を含みます。

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

* class [WorkUnit](../../workunit/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

指定された日付の作業時間量を返します。

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dt | DateTime | 作業時間を取得する対象の日付。 |

### 戻り値

指定された日の作業時間。

### 関連項目

* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


