---
title: "FontSettings.UseProjectDefaultFont"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad FontSettings. Obtiene o establece un valor que indica si se debe usar la fuente predeterminada para el renderizado."
type: docs
weight: 40
url: /es/net/aspose.tasks/fontsettings/useprojectdefaultfont/
---
## FontSettings.UseProjectDefaultFont property

Obtiene o establece un valor que indica si se debe usar la fuente predeterminada para el renderizado.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

## Observaciones

Cuando el valor es False y se especifica DefaultFontName, el motor de renderizado utilizará la fuente especificada por DefaultFontName como fuente de respaldo. De lo contrario, se usan las fuentes 'Arial' (si está instalada) o 'Generic Sans Serif' como fuente de respaldo. La fuente de respaldo se utiliza durante el renderizado de la vista del proyecto cuando un estilo de texto hace referencia a una fuente que no está instalada en el sistema operativo actual. Para un mayor control sobre la resolución de fuentes, puede usar la devolución de llamada [`FontResolveCallback`](../fontresolvecallback/).

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


