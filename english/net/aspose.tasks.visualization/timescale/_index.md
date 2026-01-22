---
title: Enum Timescale
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.Timescale enum. Defines options which specifies how to render timescale in Gantt Chart Task Usage or Resource Usage views when the project is exported to a graphic format
type: docs
weight: 3400
url: /net/aspose.tasks.visualization/timescale/
---
## Timescale enumeration

Defines options which specifies how to render timescale in Gantt Chart, Task Usage or Resource Usage views when the project is exported to a graphic format.

```csharp
public enum Timescale
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| DefinedInView | `0` | Use timescale settings defined in project view's properties: [`BottomTimescaleTier`](../../aspose.tasks/ganttchartview/bottomtimescaletier/), [`MiddleTimescaleTier`](../../aspose.tasks/ganttchartview/middletimescaletier/), [`TopTimescaleTier`](../../aspose.tasks/ganttchartview/toptimescaletier/). Valid for formats which contains view data. For example, projects which are read from MPP format. |
| Days | `1` | Predefined two-tiered timescale where minimal level of detail is one day. |
| ThirdsOfMonths | `10` | Predefined two-tiered timescale where level of detail is one third of month. |
| Months | `30` | Predefined two-tiered timescale where minimal level of detail is one month. |

## Examples

Shows how to save project as SVG file.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // set the <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> in which the document will be saved
                            PresentationFormat = PresentationFormat.GanttChart,

                            // set a value indicating whether row height should be increased to fit its content
                            FitContent = true,

                            // set the minimal time period to render. The default value is <see cref="P:Aspose.Tasks.Saving.SaveOptions.Timescale">Days</see>
                            Timescale = Timescale.ThirdsOfMonths,

                            // determines whether to use gradient brush when rendering project layout
                            // Currently using of gradient brush is not supported for rendering to SVG.
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


