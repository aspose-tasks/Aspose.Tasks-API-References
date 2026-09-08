---
title: "SvgOptions.SvgOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de SvgOptions. Inicializa una nueva instancia de la clase SvgOptions que puede usarse para guardar el proyecto en formato SVG"
type: docs
weight: 10
url: /es/net/aspose.tasks.saving/svgoptions/svgoptions/
---
## SvgOptions constructor

Inicializa una nueva instancia de la clase [`SvgOptions`](../) que puede usarse para guardar el proyecto en formato SVG.

```csharp
public SvgOptions()
```

## Ejemplos

Muestra cómo guardar el proyecto como archivo SVG.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // establece el <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> en el que se guardará el documento
                            PresentationFormat = PresentationFormat.GanttChart,

                            // establece un valor que indica si la altura de la fila debe aumentarse para ajustarse a su contenido
                            FitContent = true,

                            // establece el período de tiempo mínimo para renderizar. El valor predeterminado es <see cref="P:Aspose.Tasks.Saving.SaveOptions.Timescale">Days</see>
                            Timescale = Timescale.ThirdsOfMonths,

                            // determina si se debe usar un pincel degradado al renderizar el diseño del proyecto
                            // Actualmente, el uso de pincel degradado no es compatible con el renderizado a SVG.
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### Ver también

* class [SvgOptions](../)
* namespace [Aspose.Tasks.Saving](../../svgoptions/)
* assembly [Aspose.Tasks](../../../)


