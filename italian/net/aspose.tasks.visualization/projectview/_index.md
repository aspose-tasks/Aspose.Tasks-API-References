---
title: "Class ProjectView"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.ProjectView class. Classe di visualizzazione dei progetti."
type: docs
weight: 3300
url: /it/net/aspose.tasks.visualization/projectview/
---
## ProjectView class

Classe di visualizzazione del progetto

```csharp
public class ProjectView
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ProjectView](projectview/)(IEnumerable&lt;ViewColumn&gt;) | Inizializza una nuova istanza della classe `ProjectView`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Columns](../../aspose.tasks.visualization/projectview/columns/) { get; } | Ottiene le colonne della visualizzazione del progetto. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [GetDefaultAssignmentView](../../aspose.tasks.visualization/projectview/getdefaultassignmentview/)() | Include le colonne Uid, nome attività, nome risorsa, lavoro e durata dell'assegnazione. |
| static [GetDefaultGanttChartView](../../aspose.tasks.visualization/projectview/getdefaultganttchartview/)() | Include le colonne id, indicatori, nome, durata, inizio e fine attività. |
| static [GetDefaultResourceSheetView](../../aspose.tasks.visualization/projectview/getdefaultresourcesheetview/)() | Include le colonne Uid, nome risorsa, tipo, etichetta materiale, iniziali, gruppo, unità massime, tariffa standard, tariffa straordinaria, costo per utilizzo, accumulo a, calendario base e codice risorsa. |
| static [GetDefaultResourceUsageView](../../aspose.tasks.visualization/projectview/getdefaultresourceusageview/)() | Include le colonne Uid, nome, inizio, fine e risorsa di lavoro. |
| static [GetDefaultTaskSheetView](../../aspose.tasks.visualization/projectview/getdefaulttasksheetview/)() | Include le colonne id, indicatori, nome, durata, inizio, fine, predecessori e nomi delle risorse delle attività. |

## Esempi

Mostra come salvare un progetto con la visualizzazione delle assegnazioni.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


