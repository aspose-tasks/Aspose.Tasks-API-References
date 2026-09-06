---
title: "Calendar.Exceptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 属性。获取 CalendarExceptionCollection 对象。与日历关联的异常集合。"
type: docs
weight: 50
url: /zh/net/aspose.tasks/calendar/exceptions/
---
## Calendar.Exceptions property

获取 CalendarExceptionCollection 对象。与该日历关联的异常集合。

```csharp
public CalendarExceptionCollection Exceptions { get; }
```

## 示例

展示如何检索日历异常的信息。

```csharp
var project = new Project(DataDir + "project_RetrieveExceptions_test.mpp");

// 遍历日历
foreach (var calendar in project.Calendars)
{
    // 访问日历异常
    foreach (var exception in calendar.Exceptions)
    {
        Console.WriteLine("From: " + exception.FromDate.ToShortDateString());
        Console.WriteLine("To: " + exception.ToDate.ToShortDateString());
    }
}
```

### 另见

* class [CalendarExceptionCollection](../../calendarexceptioncollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


