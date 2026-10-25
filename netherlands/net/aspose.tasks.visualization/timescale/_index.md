---
title: "Enum Timescale"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.Timescale enum. Definieert opties die specificeren hoe de tijdschaal wordt weergegeven in Gantt-diagram Taakgebruik- of Resourcegebruik-weergaven wanneer het project wordt geëxporteerd naar een grafisch formaat."
type: docs
weight: 3430
url: /nl/net/aspose.tasks.visualization/timescale/
---
## Timescale enumeration

Definieert opties die bepalen hoe de tijdschaal wordt weergegeven in Gantt Chart, Taakgebruik of Resourcegebruik weergaven wanneer het project wordt geëxporteerd naar een grafisch formaat.

```csharp
public enum Timescale
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| DefinedInView | `0` | Gebruik tijdschaalinstellingen die zijn gedefinieerd in de eigenschappen van de projectweergave: [`BottomTimescaleTier`](../../aspose.tasks/ganttchartview/bottomtimescaletier/), [`MiddleTimescaleTier`](../../aspose.tasks/ganttchartview/middletimescaletier/), [`TopTimescaleTier`](../../aspose.tasks/ganttchartview/toptimescaletier/). Geldig voor formaten die weergavegegevens bevatten. Bijvoorbeeld projecten die uit het MPP-formaat worden gelezen. |
| Days | `1` | Vooraf gedefinieerde tweelaagse tijdschaal waarbij het minimale detailniveau één dag is. |
| ThirdsOfMonths | `10` | Vooraf gedefinieerde tweelaagse tijdschaal waarbij het detailniveau één derde van een maand is. |
| Months | `30` | Vooraf gedefinieerde tweelaagse tijdschaal waarbij het minimale detailniveau één maand is. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


