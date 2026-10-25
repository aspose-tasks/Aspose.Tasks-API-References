---
title: "CalendarCollection.Count"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CalendarCollection 属性。获取此 CalendarCollection 对象中包含的对象数量"
type: docs
weight: 10
url: /zh/net/aspose.tasks/calendarcollection/count/
---
## CalendarCollection.Count property

获取此 [`CalendarCollection`](../) 对象中包含的对象数量。

```csharp
public int Count { get; }
```

## 示例

展示如何遍历日历集合。

```csharp
var project = new Project(DataDir + "Project5.mpp");

Console.WriteLine("Number of calendars in the project: " + project.Calendars.Count);
List<Calendar> calendars = project.Calendars.ToList();
foreach (var calendar in calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### 另见

* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


