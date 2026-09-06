---
title: "Prj.WeekStartDay"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。一周的第一天"
type: docs
weight: 780
url: /zh/net/aspose.tasks/prj/weekstartday/
---
## Prj.WeekStartDay field

一周的第一天。

```csharp
public static readonly Key<DayType, PrjKey> WeekStartDay;
```

## 示例

展示如何读取/写入 项目的工作日属性。

```csharp
var project = new Project(DataDir + "WriteWeekdayProperties.mpp");

// 设置工作日属性
project.Set(Prj.WeekStartDay, DayType.Monday);
project.Set(Prj.DaysPerMonth, 24);
project.Set(Prj.MinutesPerDay, 540);
project.Set(Prj.MinutesPerWeek, 3240);

// 显示工作日属性
Console.WriteLine("Week Start Date: " + project.Get(Prj.WeekStartDay));
Console.WriteLine("Days Per Month: " + project.Get(Prj.DaysPerMonth));
Console.WriteLine("Minutes Per Day: " + project.Get(Prj.MinutesPerDay));
Console.WriteLine("Minutes Per Week: " + project.Get(Prj.MinutesPerWeek));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [DayType](../../daytype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


