---
title: "Class XlsxOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Saving.XlsxOptions. Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in XLSX"
type: docs
weight: 2270
url: /it/net/aspose.tasks.saving/xlsxoptions/
---
## XlsxOptions class

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in XLSX.

```csharp
public class XlsxOptions : SimpleSaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [XlsxOptions](xlsxoptions/)() | Inizializza una nuova istanza della classe `XlsxOptions` che può essere usata per salvare il progetto in formato XLSX. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/xlsxoptions/assignmentview/) { get; set; } | Ottiene o imposta un elenco delle colonne della vista assegnazioni da renderizzare ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [Encoding](../../aspose.tasks.saving/xlsxoptions/encoding/) { get; set; } | Ottiene o imposta la codifica del file XLSX risultante. Il valore predefinito è UTF8. |
| [ResourceView](../../aspose.tasks.saving/xlsxoptions/resourceview/) { get; set; } | Ottiene o imposta un elenco delle colonne della vista risorse da renderizzare ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Ottiene o imposta il formato in cui il documento verrà salvato se viene utilizzato questo oggetto di opzioni di salvataggio. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Ottiene o imposta il comparatore per ordinare le attività nel diagramma di Gantt e nella tabella delle attività. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Ottiene o imposta la condizione utilizzata per filtrare le attività visualizzate nei diagrammi Gantt, nella tabella delle attività e nell'utilizzo delle attività. |
| [View](../../aspose.tasks.saving/xlsxoptions/view/) { get; set; } | Ottiene o imposta un elenco delle colonne di visualizzazione ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) da salvare nel formato XLSX. Se non impostato, vengono salvate le colonne predefinite. |

## Esempi

Mostra come salvare un progetto in un file XLSX utilizzando le opzioni &lt;see cref="P:Aspose.Tasks.Saving.XlsxOptions"&gt;Days&lt;/see&gt;.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new XlsxOptions();

// Aggiungi le colonne desiderate del diagramma di Gantt
var col = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(col);

// Aggiungi le colonne desiderate della vista risorse
var rscCol = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(rscCol);

// Aggiungi le colonne desiderate della vista assegnazioni
var assnCol = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assnCol);

// imposta codifica
options.Encoding = Encoding.Unicode;

project.Save(OutDir + "UsingXlsxOptions_out.xlsx", options);
```

### Vedi anche

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


