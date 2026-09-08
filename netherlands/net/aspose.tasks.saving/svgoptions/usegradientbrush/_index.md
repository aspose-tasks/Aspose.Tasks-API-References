---
title: "SvgOptions.UseGradientBrush"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SvgOptions property. Bepaalt of een gradientborstel moet worden gebruikt bij het renderen van de projectlay-out. Het gebruik van een gradientborstel wordt momenteel niet ondersteund bij het renderen naar SVG"
type: docs
weight: 30
url: /nl/net/aspose.tasks.saving/svgoptions/usegradientbrush/
---
## SvgOptions.UseGradientBrush property

Bepaalt of een gradient‑kwast moet worden gebruikt bij het renderen van de projectlay-out. Het gebruik van een gradient‑kwast wordt momenteel niet ondersteund voor het renderen naar SVG.

```csharp
public override bool UseGradientBrush { get; set; }
```

## Voorbeelden

Toont hoe een project op te slaan als SVG‑bestand.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // stel de <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> in waarin het document zal worden opgeslagen
                            PresentationFormat = PresentationFormat.GanttChart,

                            // stel een waarde in die aangeeft of de rijhoogte moet worden vergroot om de inhoud te passen
                            FitContent = true,

                            // stel de minimale tijdsperiode in om te renderen. De standaardwaarde is <see cref="P:Aspose.Tasks.Saving.SaveOptions.Timescale">Days</see>
                            Timescale = Timescale.ThirdsOfMonths,

                            // bepaalt of een gradient‑kwast moet worden gebruikt bij het renderen van de projectlay-out
                            // Het gebruik van een gradient‑kwast wordt momenteel niet ondersteund voor het renderen naar SVG.
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### Zie ook

* class [SvgOptions](../)
* namespace [Aspose.Tasks.Saving](../../svgoptions/)
* assembly [Aspose.Tasks](../../../)


