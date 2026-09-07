---
title: "Classe Gridline"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.Gridline class. La linea orizzontale o verticale che appare nella visualizzazione del progetto"
type: docs
weight: 3100
url: /it/net/aspose.tasks.visualization/gridline/
---
## Gridline class

La linea orizzontale o verticale che appare nella visualizzazione del progetto.

```csharp
public class Gridline
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Gridline](gridline/)() | Inizializza una nuova istanza della classe `Gridline`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Color](../../aspose.tasks.visualization/gridline/color/) { get; set; } | Ottiene o imposta il [`Color`](./color/) di una gridline. |
| [GridlineType](../../aspose.tasks.visualization/gridline/gridlinetype/) { get; set; } | Ottiene o imposta il tipo di gridline ([`GridlineType`](./gridlinetype/)). |
| [Pattern](../../aspose.tasks.visualization/gridline/pattern/) { get; set; } | Ottiene o imposta il [`LinePattern`](../linepattern/) di una gridline. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.tasks.visualization/gridline/equals/)(object) | Restituisce una flag che indica se questa istanza è uguale all'oggetto specificato. |
| override [GetHashCode](../../aspose.tasks.visualization/gridline/gethashcode/)() | Restituisce un valore di codice hash per l'istanza della classe `Gridline`. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


