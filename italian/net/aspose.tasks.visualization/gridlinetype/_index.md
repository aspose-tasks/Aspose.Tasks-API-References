---
title: "Enum GridlineType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.GridlineType enum. Tipo di linea della griglia"
type: docs
weight: 3110
url: /it/net/aspose.tasks.visualization/gridlinetype/
---
## GridlineType enumeration

Tipo di linea della griglia.

```csharp
public enum GridlineType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| GanttRow | `0` | Indica la linea della griglia di una riga gantt. |
| TopTierColumn | `1` | Indica la linea della griglia di una colonna di livello superiore. |
| BottomTierColumn | `2` | Indica la linea della griglia di una colonna di livello inferiore. |
| SheetRow | `3` | Indica la linea della griglia di una riga di foglio. |
| SheetColumn | `4` | Indica la linea della griglia di una colonna di foglio. |
| UsageRow | `5` | Indica la linea della griglia di una riga di utilizzo. |
| UsageColumn | `6` | Indica la linea della griglia di una colonna di utilizzo. |
| GanttTitleVertical | `7` | Indica il tipo di linea della griglia verticale del titolo Gantt. |
| GanttTitleHorizontal | `8` | Indica il tipo di linea della griglia orizzontale del titolo Gantt. |
| BarRows | `9` | Indica il tipo di linea della griglia delle righe della barra. |
| GanttProjectStart | `10` | Indica il tipo di linea della griglia di inizio del progetto Gantt. |
| GanttProjectFinish | `11` | Indica il tipo di linea della griglia di fine del progetto Gantt. |
| GanttStatusDate | `12` | Indica il tipo di linea della griglia della data di stato del Gantt. |
| GanttCurrentDate | `13` | Indica il tipo di linea della griglia della data corrente del Gantt. |
| GanttPageBreaks | `14` | Indica il tipo di linea della griglia delle interruzioni di pagina del Gantt. |
| MiddleTierColumn | `15` | Indica il tipo di linea della griglia della colonna di livello intermedio. |

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


