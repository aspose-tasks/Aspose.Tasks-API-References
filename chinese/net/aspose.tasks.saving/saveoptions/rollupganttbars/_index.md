---
title: "SaveOptions.RollUpGanttBars"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SaveOptions 属性。获取或设置一个值，指示是否应标记汇总任务栏上的子任务。对于子任务，Rollup 字段指示子任务甘特条的信息是否会汇总到汇总任务栏。对于汇总任务，Rollup 字段指示汇总任务栏是否显示汇总后的条形。必须将汇总任务的 Rollup 字段设置为 Yes，子任务才能汇总到它们。"
type: docs
weight: 160
url: /zh/net/aspose.tasks.saving/saveoptions/rollupganttbars/
---
## SaveOptions.RollUpGanttBars property

获取或设置一个值，指示是否应在汇总任务条上标记子任务。对于子任务，Rollup 字段指示子任务甘特条的信息是否会汇总到汇总任务条。对于汇总任务，Rollup 字段指示汇总任务条是否显示已汇总的条形。必须将汇总任务的 Rollup 字段设置为 Yes，子任务才能汇总到它们上。

```csharp
public bool RollUpGanttBars { get; set; }
```

## 备注

仅在渲染甘特图视图时适用。

## 示例

展示如何设置一个值，指示汇总任务栏上的子任务必须向上汇总。

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // 或
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### 另见

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


