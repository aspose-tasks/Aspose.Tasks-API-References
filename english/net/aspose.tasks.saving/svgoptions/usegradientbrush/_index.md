---
title: SvgOptions.UseGradientBrush
second_title: Aspose.Tasks for .NET API Reference
description: SvgOptions property. Determines whether to use gradient brush when rendering project layout. Currently using of gradient brush is not supported for rendering to SVG
type: docs
weight: 30
url: /net/aspose.tasks.saving/svgoptions/usegradientbrush/
---
## SvgOptions.UseGradientBrush property

Determines whether to use gradient brush when rendering project layout. Currently using of gradient brush is not supported for rendering to SVG.

```csharp
public override bool UseGradientBrush { get; set; }
```

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

* class [SvgOptions](../)
* namespace [Aspose.Tasks.Saving](../../svgoptions/)
* assembly [Aspose.Tasks](../../../)


