---
title: "Class Gridlines"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.Gridlines classe. Rappresenta le linee della griglia che appaiono in una visualizzazione GanttChart."
type: docs
weight: 3120
url: /it/net/aspose.tasks.visualization/gridlines/
---
## Gridlines class

Rappresenta le linee della griglia che appaiono in una visualizzazione GanttChart.

```csharp
public class Gridlines
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Gridlines](gridlines/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Interval](../../aspose.tasks.visualization/gridlines/interval/) { get; set; } | Ottiene o imposta il numero da 0 a 99 che specifica l'intervallo tra le linee della griglia. |
| [IntervalColor](../../aspose.tasks.visualization/gridlines/intervalcolor/) { get; set; } | Ottiene o imposta il colore delle linee della griglia secondarie. |
| [IntervalPattern](../../aspose.tasks.visualization/gridlines/intervalpattern/) { get; set; } | Ottiene o imposta il modello di linea per le linee della griglia secondarie. |
| [NormalColor](../../aspose.tasks.visualization/gridlines/normalcolor/) { get; set; } | Ottiene o imposta il colore delle linee della griglia normali. |
| [NormalPattern](../../aspose.tasks.visualization/gridlines/normalpattern/) { get; set; } | Ottiene o imposta il modello di linea per le linee della griglia normali. |
| [Type](../../aspose.tasks.visualization/gridlines/type/) { get; set; } | Ottiene o imposta il tipo di linea della griglia. |

## Esempi

Mostra come lavorare con le linee della griglia.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var view = (GanttChartView)project.Views.ToList()[0];

// consente di regolare la prima linea della griglia della vista
var gridlines = view.Gridlines[0];
// imposta il numero da 0 a 99 che specifica l'intervallo tra le linee della griglia.
gridlines.Interval = 2;
// imposta il colore delle linee della griglia secondarie.
gridlines.IntervalColor = Color.Red;
// imposta il modello di linea per le linee della griglia secondarie
gridlines.IntervalPattern = LinePattern.Solid;
// imposta il colore delle linee della griglia normali
gridlines.NormalColor = Color.Blue;
// imposta il modello di linea per le linee della griglia normali
gridlines.NormalPattern = LinePattern.CloseDot;
// imposta il tipo di linea della griglia
gridlines.Type = GridlineType.GanttRow;

project.Save(OutDir + "WorkWithGridlines_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


