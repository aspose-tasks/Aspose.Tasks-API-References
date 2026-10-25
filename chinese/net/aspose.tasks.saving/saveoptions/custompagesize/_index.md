---
title: "SaveOptions.CustomPageSize"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SaveOptions 属性。获取或设置自定义页面大小（单位为点），1 点 = 1/72 英寸。"
type: docs
weight: 20
url: /zh/net/aspose.tasks.saving/saveoptions/custompagesize/
---
## SaveOptions.CustomPageSize property

获取或设置自定义页面大小（单位为点，1 点 = 1/72 英寸）。

```csharp
public SizeF CustomPageSize { get; set; }
```

## 示例

展示如何在项目保存为 PDF 时设置自定义页面大小。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.GanttChart;
options.CustomPageSize = new SizeF(5.8F * 72, 8.3F * 72);

project.Save(OutDir + "WorkWithCustomPageSize_out.pdf", options);
```

### 另见

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


