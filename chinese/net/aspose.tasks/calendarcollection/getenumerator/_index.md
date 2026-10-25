---
title: "CalendarCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CalendarCollection 方法。返回此集合的枚举器"
type: docs
weight: 50
url: /zh/net/aspose.tasks/calendarcollection/getenumerator/
---
## CalendarCollection.GetEnumerator method

返回此集合的枚举器。

```csharp
public IEnumerator<Calendar> GetEnumerator()
```

### 返回值

此集合的枚举器。

## 示例

展示如何添加新日历。

```csharp
var project = new Project();

// 可以通过使用集合的 Add 重载向项目的日历集合添加新日历。
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### 另见

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


