---
title: "FontSettings.DefaultFontName"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad FontSettings. Obtiene o establece la fuente predeterminada o de respaldo para el renderizado."
type: docs
weight: 20
url: /es/net/aspose.tasks/fontsettings/defaultfontname/
---
## FontSettings.DefaultFontName property

Obtiene o establece la fuente predeterminada (o de respaldo) para el renderizado.

```csharp
public string DefaultFontName { get; set; }
```

## Ejemplos

Muestra cómo establecer una fuente personalizada que se usará para imprimir el PDF de salida.

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

### Ver también

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


