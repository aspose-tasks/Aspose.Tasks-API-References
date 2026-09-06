---
title: "SaveOptions.IsPortrait"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SaveOptions 属性。获取或设置一个值，指示页面方向是否为纵向，如果页面方向为横向则返回 false。"
type: docs
weight: 70
url: /zh/net/aspose.tasks.saving/saveoptions/isportrait/
---
## SaveOptions.IsPortrait property

获取或设置一个值，指示页面方向是否为纵向；如果页面方向为横向，则返回 false。

```csharp
public bool IsPortrait { get; set; }
```

## 备注

当 SaveOptions.PageSize == Visualization.PageSize.DefinedInView 时不适用。在这种情况下使用 View.PageInfo.PageSettings.IsPortrait。 当 SaveOptions.CustomPageSize 已设置时也不适用。

## 示例

展示如何使用 View 设置或使用 SaveOptions 指定页面大小和方向。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// 在这种情况下，页面大小和方向取自 view.PageInfo.PageSettings.PaperSize 和 view.PageInfo.PageSettings.IsPortrait 属性。
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// 在这种情况下，页面大小和方向取自 SaveOptions 的属性。
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// 在这种情况下，页面大小取自 SaveOptions.CustomPageSize。IsPortrait 属性不予考虑。
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### 另见

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


