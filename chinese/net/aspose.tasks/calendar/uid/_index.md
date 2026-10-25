---
title: "Calendar.Uid"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 属性。获取或设置日历的唯一标识符"
type: docs
weight: 110
url: /zh/net/aspose.tasks/calendar/uid/
---
## Calendar.Uid property

获取或设置日历的唯一标识符。

```csharp
public int Uid { get; set; }
```

## 示例

展示如何检索日历信息。

```csharp
var project = new Project(DataDir + "RetrieveCalendarInfo.mpp");

// 检索日历信息
foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("Calendar UID: " + calendar.Uid);
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### 另见

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


