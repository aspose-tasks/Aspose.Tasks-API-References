---
title: "HtmlSaveOptions.UseGradientBrush"
second_title: "Aspose.Tasks for .NET API 参考"
description: "HtmlSaveOptions 属性。获取或设置一个值，指示在渲染项目布局时是否使用渐变画刷。目前在渲染为 HTML 时不支持使用渐变画刷。"
type: docs
weight: 160
url: /zh/net/aspose.tasks.saving/htmlsaveoptions/usegradientbrush/
---
## HtmlSaveOptions.UseGradientBrush property

获取或设置指示在渲染项目布局时是否使用渐变画刷的值。目前在渲染为 HTML 时不支持使用渐变画刷。

```csharp
public override bool UseGradientBrush { get; set; }
```

## 示例

展示如何设置将在 HTML 文件中导出项目时使用的自定义字体。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart,
                      FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "AddDefaultFontDuringSavingAsHtml_out.html", options);
```

### 另见

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


