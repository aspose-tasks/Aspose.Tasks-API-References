---
title: "SaveOptions.PageSize"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SaveOptions 属性。获取或设置要渲染的页面大小，默认值为 PageSize.A4"
type: docs
weight: 130
url: /zh/net/aspose.tasks.saving/saveoptions/pagesize/
---
## SaveOptions.PageSize property

获取或设置要渲染的页面大小（默认值为 PageSize.A4）。

```csharp
public PageSize PageSize { get; set; }
```

## 示例

展示如何设置页面大小（可以是 &lt;see cref="P:Aspose.Tasks.Visualization.TiffCompression" /&gt; 枚举的其中一个值）。

```csharp
var project = new Project(DataDir + "Project2.mpp");

const PresentationFormat format = PresentationFormat.GanttChart;

// 将项目渲染为所有预定义的页面大小
foreach (var pageSize in (PageSize[])Enum.GetValues(typeof(PageSize)))
{
    var options = new PdfSaveOptions
    {
        PresentationFormat = format,
        FitContent = true,
        PageSize = pageSize
    };
    project.Save(OutDir + "PredefinedPageSizes_" + format + "_" + pageSize + "_out.pdf", options);
}
```

### 另见

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


