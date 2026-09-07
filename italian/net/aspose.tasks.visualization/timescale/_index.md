---
title: "Enum Timescale"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.Timescale enum. Definisce le opzioni che specificano come rendere la scala temporale nelle viste Gantt Chart Task Usage o Resource Usage quando il progetto viene esportato in un formato grafico."
type: docs
weight: 3430
url: /it/net/aspose.tasks.visualization/timescale/
---
## Timescale enumeration

Definisce le opzioni che specificano come visualizzare la scala temporale in Gantt Chart, Task Usage o Resource Usage quando il progetto viene esportato in un formato grafico.

```csharp
public enum Timescale
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| DefinedInView | `0` | Utilizza le impostazioni della scala temporale definite nelle proprietà della vista del progetto: [`BottomTimescaleTier`](../../aspose.tasks/ganttchartview/bottomtimescaletier/), [`MiddleTimescaleTier`](../../aspose.tasks/ganttchartview/middletimescaletier/), [`TopTimescaleTier`](../../aspose.tasks/ganttchartview/toptimescaletier/). Valido per i formati che contengono dati della vista. Ad esempio, progetti letti dal formato MPP. |
| Days | `1` | Scala temporale a due livelli predefinita in cui il livello minimo di dettaglio è un giorno. |
| ThirdsOfMonths | `10` | Scala temporale a due livelli predefinita in cui il livello di dettaglio è un terzo di mese. |
| Months | `30` | Scala temporale a due livelli predefinita in cui il livello minimo di dettaglio è un mese. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


