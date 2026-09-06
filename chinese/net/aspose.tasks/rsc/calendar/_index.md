---
title: "Rsc.Calendar"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源的日历"
type: docs
weight: 190
url: /zh/net/aspose.tasks/rsc/calendar/
---
## Rsc.Calendar field

资源的日历。

```csharp
public static readonly Key<Calendar, RscKey> Calendar;
```

## 示例

展示如何获取/设置资源日历。

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var res = project.Resources.Add("Resource1");

// 添加标准日历并分配给资源
var cal = project.Calendars.Add("Resource1");
res.Set(Rsc.Calendar, cal);

// 显示所有资源的基础日历名称
foreach (var resource in project.Resources)
{
    if (resource.Get(Rsc.Name) != null)
    {
        Console.WriteLine(resource.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


