---
title: "ProjectView.GetDefaultTaskSheetView"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ProjectView. Include gli indicatori id, nome, durata, inizio, fine, predecessori e nomi delle risorse nelle colonne delle attività"
type: docs
weight: 60
url: /it/net/aspose.tasks.visualization/projectview/getdefaulttasksheetview/
---
## ProjectView.GetDefaultTaskSheetView method

Include le colonne id, indicatori, nome, durata, inizio, fine, predecessori e nomi delle risorse delle attività.

```csharp
public static ProjectView GetDefaultTaskSheetView()
```

### Valore di ritorno

una vista che contiene un elenco di [`GanttChartColumn`](../../ganttchartcolumn/).

## Esempi

Mostra come salvare un progetto con la vista task sheet.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultTaskSheetView()
};

project.Save(OutDir + "WorkWithProjectView_TaskSheetView_out.pdf", options);
```

### Vedi anche

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


