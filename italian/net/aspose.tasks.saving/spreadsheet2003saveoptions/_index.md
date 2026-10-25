---
title: "Classe Spreadsheet2003SaveOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Saving.Spreadsheet2003SaveOptions. Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in Spreadsheet2003"
type: docs
weight: 2220
url: /it/net/aspose.tasks.saving/spreadsheet2003saveoptions/
---
## Spreadsheet2003SaveOptions class

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in Spreadsheet2003.

```csharp
public class Spreadsheet2003SaveOptions : SimpleSaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Spreadsheet2003SaveOptions](spreadsheet2003saveoptions/)() | Inizializza una nuova istanza della classe `Spreadsheet2003SaveOptions`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/spreadsheet2003saveoptions/assignmentview/) { get; set; } | Ottiene o imposta un elenco delle colonne della vista assegnazioni da renderizzare ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [ResourceView](../../aspose.tasks.saving/spreadsheet2003saveoptions/resourceview/) { get; set; } | Ottiene o imposta un elenco delle colonne della vista risorse da renderizzare ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Ottiene o imposta il formato in cui il documento verrà salvato se viene utilizzato questo oggetto di opzioni di salvataggio. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Ottiene o imposta il comparatore per ordinare le attività nel diagramma di Gantt e nella tabella delle attività. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Ottiene o imposta la condizione utilizzata per filtrare le attività visualizzate nei diagrammi Gantt, nella tabella delle attività e nell'utilizzo delle attività. |
| [View](../../aspose.tasks.saving/spreadsheet2003saveoptions/view/) { get; set; } | Ottiene o imposta un elenco delle colonne della vista ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) da salvare. Se non impostato, vengono salvate le colonne predefinite. |

## Esempi

Mostra come aggiungere colonne da esportare durante l'esportazione del progetto nel formato Spreadsheet2003.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();
var ganttChartColumn = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(ganttChartColumn);

var resourceViewColumn = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(resourceViewColumn);

var assignmentViewColumn = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assignmentViewColumn);

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### Vedi anche

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


