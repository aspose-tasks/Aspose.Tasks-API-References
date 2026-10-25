---
title: "SvgOptions.UseGradientBrush"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SvgOptions. Determina se utilizzare un pennello gradiente durante il rendering del layout del progetto. Attualmente l'uso del pennello gradiente non è supportato per il rendering in SVG"
type: docs
weight: 30
url: /it/net/aspose.tasks.saving/svgoptions/usegradientbrush/
---
## SvgOptions.UseGradientBrush property

Determina se utilizzare un pennello gradiente durante il rendering del layout del progetto. Attualmente l'uso del pennello gradiente non è supportato per il rendering in SVG.

```csharp
public override bool UseGradientBrush { get; set; }
```

## Esempi

Mostra come salvare il progetto come file SVG.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // imposta il <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> in cui il documento sarà salvato
                            PresentationFormat = PresentationFormat.GanttChart,

                            // imposta un valore che indica se l'altezza della riga deve essere aumentata per adattarsi al contenuto
                            FitContent = true,

                            // imposta il periodo di tempo minimo da renderizzare. Il valore predefinito è <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.Timescale\">Days</see>
                            Timescale = Timescale.ThirdsOfMonths,

                            // determina se utilizzare un pennello gradiente durante il rendering del layout del progetto
                            // Attualmente l'uso del pennello gradiente non è supportato per il rendering in SVG.
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### Vedi anche

* class [SvgOptions](../)
* namespace [Aspose.Tasks.Saving](../../svgoptions/)
* assembly [Aspose.Tasks](../../../)


