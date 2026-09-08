---
title: "HtmlSaveOptions.UseGradientBrush"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad HtmlSaveOptions. Obtiene o establece un valor que indica si se debe usar un pincel degradado al renderizar el diseño del proyecto. Actualmente, el uso de pincel degradado no es compatible al renderizar a HTML"
type: docs
weight: 160
url: /es/net/aspose.tasks.saving/htmlsaveoptions/usegradientbrush/
---
## HtmlSaveOptions.UseGradientBrush property

Obtiene o establece un valor que indica si se debe usar un pincel degradado al renderizar el diseño del proyecto. Actualmente, el uso de pincel degradado no es compatible al renderizar a HTML.

```csharp
public override bool UseGradientBrush { get; set; }
```

## Ejemplos

Muestra cómo establecer una fuente personalizada que se utilizará para exportar el proyecto en un archivo HTML.

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

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


