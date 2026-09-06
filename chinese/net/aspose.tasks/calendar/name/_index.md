---
title: "Calendar.Name"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 属性。获取或设置日历的名称"
type: docs
weight: 90
url: /zh/net/aspose.tasks/calendar/name/
---
## Calendar.Name property

获取或设置日历的名称。

```csharp
public string Name { get; set; }
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


