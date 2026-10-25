---
title: "CalendarException.Delete"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CalendarException 方法。删除父日历 CalendarExceptionCollection 对象中的 Exception 实例。"
type: docs
weight: 180
url: /zh/net/aspose.tasks/calendarexception/delete/
---
## CalendarException.Delete method

从父日历 CalendarExceptionCollection 对象中删除 Exception 实例。

```csharp
public void Delete()
```

## 示例

展示如何删除日历异常。

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);

// 删除该异常。
calendar.Exceptions[0].Delete();

Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
```

### 另见

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


