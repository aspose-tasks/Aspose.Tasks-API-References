---
title: "CalendarCollection.ToList"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CalendarCollection 方法。将 CalendarCollection 对象转换为 Calendar 对象列表"
type: docs
weight: 70
url: /zh/net/aspose.tasks/calendarcollection/tolist/
---
## CalendarCollection.ToList method

将 CalendarCollection 对象转换为 [`Calendar`](../../calendar/) 对象列表。

```csharp
public List<Calendar> ToList()
```

### 返回值

[`Calendar`](../../calendar/) 对象列表。

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

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


