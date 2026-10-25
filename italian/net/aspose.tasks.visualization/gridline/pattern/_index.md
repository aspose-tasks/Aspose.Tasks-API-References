---
title: "Gridline.Pattern"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Gridline. Ottiene o imposta il LinePattern di una linea di griglia"
type: docs
weight: 40
url: /it/net/aspose.tasks.visualization/gridline/pattern/
---
## Gridline.Pattern property

Ottiene o imposta il [`LinePattern`](../../linepattern/) di una linea di griglia.

```csharp
public LinePattern Pattern { get; set; }
```

## Esempi

Mostra come lavorare con le linee della griglia durante il salvataggio in formati visuali.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // imposta il tipo di linea della griglia (<see cref=\"P:Aspose.Tasks.Visualization.Gridline.GridlineType\" />).
    GridlineType = GridlineType.GanttRow, 
    // imposta il <see cref=\"T:Aspose.Tasks.Visualization.LinePattern\" /> di una linea della griglia
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### Vedi anche

* enum [LinePattern](../../linepattern/)
* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


