---
title: HtmlSaveOptions.UseGradientBrush
second_title: Aspose.Tasks for .NET API Reference
description: HtmlSaveOptions property. Gets or sets a value indicating whether to use gradient brush when rendering project layout. Currently using of gradient brush is not supported when rendering to HTML
type: docs
weight: 160
url: /net/aspose.tasks.saving/htmlsaveoptions/usegradientbrush/
---
## HtmlSaveOptions.UseGradientBrush property

Gets or sets a value indicating whether to use gradient brush when rendering project layout. Currently using of gradient brush is not supported when rendering to HTML.

```csharp
public override bool UseGradientBrush { get; set; }
```

## Examples

Shows how to set custom font that will be used to export the project in HTML file.

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

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


