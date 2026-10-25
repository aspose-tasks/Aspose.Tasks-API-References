---
title: "FontSettings.DefaultFontName"
second_title: "Aspose.Tasks for .NET API 参考"
description: "FontSettings 属性。获取或设置渲染时的默认或回退字体"
type: docs
weight: 20
url: /zh/net/aspose.tasks/fontsettings/defaultfontname/
---
## FontSettings.DefaultFontName property

获取或设置渲染时的默认（或回退）字体。

```csharp
public string DefaultFontName { get; set; }
```

## 示例

展示如何设置将在输出 PDF 打印时使用的自定义字体。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### 另见

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


