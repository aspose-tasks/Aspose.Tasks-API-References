---
title: "Calendar.BaseCalendar"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 属性。获取或设置此日历所依赖的基础日历。仅在该日历不是基础日历时适用。"
type: docs
weight: 40
url: /zh/net/aspose.tasks/calendar/basecalendar/
---
## Calendar.BaseCalendar property

获取或设置此日历所依赖的基础日历。仅在该日历不是基础日历时适用。

```csharp
public Calendar BaseCalendar { get; set; }
```

## 示例

展示如何使用资源日历的基础日历。

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var resource = project.Resources.Add("Resource1");

// 添加标准日历并分配给资源
var calendar = project.Calendars.Add("Resource1");
resource.Set(Rsc.Calendar, calendar);

// 显示所有资源的基础日历名称
foreach (var rsc in project.Resources)
{
    if (rsc.Get(Rsc.Name) != null)
    {
        Console.WriteLine(rsc.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### 另见

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


