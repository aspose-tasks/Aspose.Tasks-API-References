---
title: "SaveOptions.ViewSettings"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SaveOptions 属性。获取或设置要渲染的视图 View。您可以使用此选项显式指定应保存为 PDF、HTML 或图像格式的视图。如果设置了此属性，保存项目时会忽略 PresentationFormat 属性。View 必须来自以下其中一个 screen：Screen、Gantt、TaskSheet、TaskUsage、ResourceSheet、ResourceUsage。"
type: docs
weight: 240
url: /zh/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

获取或设置要渲染的视图 ([`View`](../view/))。您可以使用此选项显式指定应保存为 PDF、HTML 或图像格式的视图。如果设置了此属性，[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) 属性在保存项目时会被忽略。View 必须来自以下其中一个 screen (([`Screen`](../../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)。

```csharp
public View ViewSettings { get; set; }
```

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentException | 当调用 set 方法且提供的 View 类实例的 Screen 属性值不受支持时。 |

## 示例

展示如何使用 'SaveOptions.ViewSettings' 指定应渲染为 PDF 的视图。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);
Console.WriteLine("Page size specified in view settings: " + view.PageInfo.PageSettings.PaperSize);
Console.WriteLine("Page orientation: {0}", view.PageInfo.PageSettings.IsPortrait ? "Portrait" : "Landscape");

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.DefinedInView;
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

project.Save(OutDir + "SaveToPdfUsingSpecificView_out.pdf", saveOptions);
```

### 另见

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


