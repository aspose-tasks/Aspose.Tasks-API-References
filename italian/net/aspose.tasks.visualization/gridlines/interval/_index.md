---
title: "Gridlines.Interval"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Gridlines. Ottiene o imposta il numero da 0 a 99 che specifica l'intervallo tra le linee della griglia"
type: docs
weight: 20
url: /it/net/aspose.tasks.visualization/gridlines/interval/
---
## Gridlines.Interval property

Ottiene o imposta il numero da 0 a 99 che specifica l'intervallo tra le linee della griglia.

```csharp
public int Interval { get; set; }
```

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

* class [Gridlines](../)
* namespace [Aspose.Tasks.Visualization](../../gridlines/)
* assembly [Aspose.Tasks](../../../)


