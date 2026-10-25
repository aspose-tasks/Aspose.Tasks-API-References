---
title: "XamlOptions.XamlOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "XamlOptions 构造函数。初始化一个新的 XamlOptions 类实例，可用于以 XAML 格式保存项目"
type: docs
weight: 10
url: /zh/net/aspose.tasks.saving/xamloptions/xamloptions/
---
## XamlOptions constructor

初始化一个新的 [`XamlOptions`](../) 类实例，可用于以 XAML 格式保存项目。

```csharp
public XamlOptions()
```

## 示例

展示如何使用保存选项将项目保存为 XAML 格式。

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new XamlOptions();
options.FitContent = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "RenderXAMLWithOptions_out.xaml", options);
```

### 另见

* class [XamlOptions](../)
* namespace [Aspose.Tasks.Saving](../../xamloptions/)
* assembly [Aspose.Tasks](../../../)


