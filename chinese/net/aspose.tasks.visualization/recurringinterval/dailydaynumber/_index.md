---
title: "RecurringInterval.DailyDayNumber"
second_title: "Aspose.Tasks for .NET API 参考"
description: "RecurringInterval 属性。获取或设置每日天数"
type: docs
weight: 20
url: /zh/net/aspose.tasks.visualization/recurringinterval/dailydaynumber/
---
## RecurringInterval.DailyDayNumber property

获取或设置每日的天数。

```csharp
public int DailyDayNumber { get; set; }
```

## 示例

展示如何添加每日循环间隔的进度线。

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

view.ProgressLines.RecurringInterval = new RecurringInterval();
// 设置每日模式的天数
view.ProgressLines.RecurringInterval.DailyDayNumber = 2;
// 设置一个值，指示某天是否为每日进度线的工作日。
view.ProgressLines.RecurringInterval.DailyWorkday = true;
```

### 另见

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


