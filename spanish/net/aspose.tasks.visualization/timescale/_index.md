---
title: "Enum Timescale"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Visualization.Timescale enum. Define opciones que especifican cómo renderizar la escala de tiempo en las vistas de Uso de Tareas o Uso de Recursos del Diagrama de Gantt cuando el proyecto se exporta a un formato gráfico."
type: docs
weight: 3430
url: /es/net/aspose.tasks.visualization/timescale/
---
## Timescale enumeration

Define opciones que especifican cómo renderizar la escala de tiempo en el Diagrama de Gantt, vistas de Uso de tareas o Uso de recursos cuando el proyecto se exporta a un formato gráfico.

```csharp
public enum Timescale
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| DefinedInView | `0` | Utilice la configuración de escala de tiempo definida en las propiedades de la vista del proyecto: [`BottomTimescaleTier`](../../aspose.tasks/ganttchartview/bottomtimescaletier/), [`MiddleTimescaleTier`](../../aspose.tasks/ganttchartview/middletimescaletier/), [`TopTimescaleTier`](../../aspose.tasks/ganttchartview/toptimescaletier/). Válido para formatos que contienen datos de la vista. Por ejemplo, proyectos que se leen del formato MPP. |
| Days | `1` | Escala de tiempo de dos niveles predefinida donde el nivel mínimo de detalle es un día. |
| ThirdsOfMonths | `10` | Escala de tiempo de dos niveles predefinida donde el nivel de detalle es un tercio de mes. |
| Months | `30` | Escala de tiempo de dos niveles predefinida donde el nivel mínimo de detalle es un mes. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


