---
title: "SaveOptions.UseGradientBrush"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SaveOptions 属性。获取或设置一个值，指示在渲染甘特图时是否应使用渐变画笔"
type: docs
weight: 220
url: /zh/net/aspose.tasks.saving/saveoptions/usegradientbrush/
---
## SaveOptions.UseGradientBrush property

获取或设置指示在渲染甘特图时是否应使用渐变画刷的值。

```csharp
public virtual bool UseGradientBrush { get; set; }
```

## 备注

仅在渲染甘特图视图时适用。

## 示例

展示如何设置一个值，以指示在渲染甘特图时是否应使用渐变画笔。

```csharp
var project = new Project(DataDir + "Project2.mpp");

SaveOptions options = new XamlOptions
{
    UseGradientBrush = false
};
project.Save(OutDir + "ChangeGanttBarsColorGradient_Solid_out.xaml", options);

options.UseGradientBrush = true;
project.Save(OutDir + "ChangeGanttBarsColorGradient_Gradient_out.xaml", options);
```

### 另见

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


