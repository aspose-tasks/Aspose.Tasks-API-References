---
title: UseProjectDefaultFont
second_title: Aspose.Tasks for .NET API Reference
description: Gets or sets a value indicating whether the default font must be used for rendering.
type: docs
weight: 180
url: /net/aspose.tasks.saving/htmlsaveoptions/useprojectdefaultfont/
---
## HtmlSaveOptions.UseProjectDefaultFont property

Gets or sets a value indicating whether the default font must be used for rendering.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

### Remarks

When the value is False and DefaultFontName is specified, the rendering engine will utilize the font specified by DefaultFontName as a fallback font. Otherwise 'Arial' (if installed) or 'Generic Sans Serif' fonts are used as a fallback font. The fallback font is utilized during the rendering of project view when a text style references a font that is not installed on the current operating system. For greater control over font resolution you can use [`FontResolveCallback`](../fontresolvecallback) callback.

### Examples

Shows how to set custom font that will be used to export the project in HTML file.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart,
                      FitContent = true,
                      UseProjectDefaultFont = false,
                      DefaultFontName = "Segoe UI Black"
                  };
project.Save(OutDir + "AddDefaultFontDuringSavingAsHtml_out.html", options);
```

### See Also

* class [HtmlSaveOptions](../../htmlsaveoptions)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
