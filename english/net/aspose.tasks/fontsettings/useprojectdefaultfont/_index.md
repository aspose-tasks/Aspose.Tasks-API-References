---
title: FontSettings.UseProjectDefaultFont
second_title: Aspose.Tasks for .NET API Reference
description: FontSettings property. Gets or sets a value indicating whether the default font must be used for rendering
type: docs
weight: 40
url: /net/aspose.tasks/fontsettings/useprojectdefaultfont/
---
## FontSettings.UseProjectDefaultFont property

Gets or sets a value indicating whether the default font must be used for rendering.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

## Remarks

When the value is False and DefaultFontName is specified, the rendering engine will utilize the font specified by DefaultFontName as a fallback font. Otherwise 'Arial' (if installed) or 'Generic Sans Serif' fonts are used as a fallback font. The fallback font is utilized during the rendering of project view when a text style references a font that is not installed on the current operating system. For greater control over font resolution you can use [`FontResolveCallback`](../fontresolvecallback/) callback.

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


