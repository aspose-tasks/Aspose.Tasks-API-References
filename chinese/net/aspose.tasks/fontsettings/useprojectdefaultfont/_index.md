---
title: "FontSettings.UseProjectDefaultFont"
second_title: "Aspose.Tasks for .NET API 参考"
description: "FontSettings 属性。获取或设置一个值，指示是否必须在渲染时使用默认字体"
type: docs
weight: 40
url: /zh/net/aspose.tasks/fontsettings/useprojectdefaultfont/
---
## FontSettings.UseProjectDefaultFont property

获取或设置一个值，指示是否必须使用默认字体进行渲染。

```csharp
public bool UseProjectDefaultFont { get; set; }
```

## 备注

当值为 False 且指定了 DefaultFontName 时，渲染引擎将使用 DefaultFontName 指定的字体作为回退字体。否则将使用 'Arial'（如果已安装）或 'Generic Sans Serif' 字体作为回退字体。回退字体在项目视图渲染时使用，当文本样式引用的字体未在当前操作系统上安装时使用。若需更精细地控制字体解析，可使用 [`FontResolveCallback`](../fontresolvecallback/) 回调。

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


