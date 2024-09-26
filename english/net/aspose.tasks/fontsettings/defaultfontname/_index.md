---
title: FontSettings.DefaultFontName
second_title: Aspose.Tasks for .NET API Reference
description: FontSettings property. Gets or sets the default or fallback font for rendering
type: docs
weight: 20
url: /net/aspose.tasks/fontsettings/defaultfontname/
---
## FontSettings.DefaultFontName property

Gets or sets the default (or fallback) font for rendering.

```csharp
public string DefaultFontName { get; set; }
```

## Examples

Shows how to set custom font that will be used for print of output pdf.

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

### See Also

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


