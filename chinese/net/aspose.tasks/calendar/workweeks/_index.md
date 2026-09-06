---
title: "Calendar.WorkWeeks"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 属性。获取 WorkWeekCollections 对象。该集合包含与日历关联的工作周。"
type: docs
weight: 130
url: /zh/net/aspose.tasks/calendar/workweeks/
---
## Calendar.WorkWeeks property

获取 WorkWeekCollections 对象。与该日历关联的工作周集合。

```csharp
public WorkWeekCollection WorkWeeks { get; }
```

## 示例

展示如何读取工作周信息。

```csharp
var project = new Project(DataDir + "WorkWithWorkWeekCollection.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var workWeek in calendar.WorkWeeks)
{
    // 显示工作周名称、起始日期和结束日期。
    var name = workWeek.Name;
    var fromDate = workWeek.FromDate;
    var toDate = workWeek.ToDate;
    Console.WriteLine("Name: " + name);
    Console.WriteLine("From Date: " + fromDate);
    Console.WriteLine("To Date: " + toDate);

    // 此数据全部关于 "Details." 按钮，您可以为特定的 WeekDay 设置特殊工作时间，甚至将其设为非工作日。
    foreach (var day in workWeek.WeekDays)
    {
        // 您可以进一步遍历工作时间并显示它们。
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}
```

### 另见

* class [WorkWeekCollection](../../workweekcollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


