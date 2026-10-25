---
title: "SvgOptions.SvgOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SvgOptions constructor. Initialiseert een nieuw exemplaar van de SvgOptions-klasse die kan worden gebruikt om een project op te slaan in SVG-formaat"
type: docs
weight: 10
url: /nl/net/aspose.tasks.saving/svgoptions/svgoptions/
---
## SvgOptions constructor

Initialiseert een nieuw exemplaar van de [`SvgOptions`](../) klasse die kan worden gebruikt om een project op te slaan in SVG-formaat.

```csharp
public SvgOptions()
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


