---
title: XamlOptions.XamlOptions
second_title: Aspose.Tasks for .NET API Reference
description: XamlOptions constructor. Initializes a new instance of the XamlOptions class that can be used to save project in XAML format
type: docs
weight: 10
url: /net/aspose.tasks.saving/xamloptions/xamloptions/
---
## XamlOptions constructor

Initializes a new instance of the [`XamlOptions`](../) class that can be used to save project in XAML format.

```csharp
public XamlOptions()
```

## Examples

Shows how to save a project in XAML format by using save options.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new XamlOptions();
options.FitContent = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "RenderXAMLWithOptions_out.xaml", options);
```

### See Also

* class [XamlOptions](../)
* namespace [Aspose.Tasks.Saving](../../xamloptions/)
* assembly [Aspose.Tasks](../../../)


