---
title: SaveOptions.UseGradientBrush
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets a value indicating whether gradient brush should be used when rendering Gantt Chart
type: docs
weight: 220
url: /net/aspose.tasks.saving/saveoptions/usegradientbrush/
---
## SaveOptions.UseGradientBrush property

Gets or sets a value indicating whether gradient brush should be used when rendering Gantt Chart.

```csharp
public virtual bool UseGradientBrush { get; set; }
```

## Remarks

Is only applicable when Gantt chart view is rendered.

## Examples

shows how to set a value indicating whether gradient brush should be used when rendering Gantt Chart.

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

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


