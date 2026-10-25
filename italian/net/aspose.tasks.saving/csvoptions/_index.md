---
title: "Classe CsvOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Saving.CsvOptions. Consente di specificare opzioni aggiuntive durante il salvataggio del progetto in CSV"
type: docs
weight: 1980
url: /it/net/aspose.tasks.saving/csvoptions/
---
## CsvOptions class

Consente di specificare opzioni aggiuntive durante il salvataggio del progetto in CSV.

```csharp
public class CsvOptions : SimpleSaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [CsvOptions](csvoptions/)() | Inizializza una nuova istanza della classe `CsvOptions` che può essere utilizzata per salvare il progetto in formato CSV. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DataCategory](../../aspose.tasks.saving/csvoptions/datacategory/) { get; set; } | Ottiene o imposta una categoria di dati da salvare. |
| [Encoding](../../aspose.tasks.saving/csvoptions/encoding/) { get; set; } | Ottiene o imposta una codifica con cui salvare il CSV. |
| [IncludeHeaders](../../aspose.tasks.saving/csvoptions/includeheaders/) { get; set; } | Ottiene o imposta un valore che indica se includere le intestazioni o meno (il valore predefinito è TRUE). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Ottiene o imposta il formato in cui il documento verrà salvato se viene utilizzato questo oggetto di opzioni di salvataggio. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Ottiene o imposta il comparatore per ordinare le attività nel diagramma di Gantt e nella tabella delle attività. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Ottiene o imposta la condizione utilizzata per filtrare le attività visualizzate nei diagrammi Gantt, nella tabella delle attività e nell'utilizzo delle attività. |
| [TextDelimiter](../../aspose.tasks.saving/csvoptions/textdelimiter/) { get; set; } | Ottiene o imposta un delimitatore di testo. |
| [View](../../aspose.tasks.saving/csvoptions/view/) { get; set; } | Ottiene o imposta un elenco delle colonne di visualizzazione ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) da salvare nel formato XLSX. Se non impostato, vengono salvate le colonne predefinite. |

## Esempi

Mostra come utilizzare &lt;see cref="Aspose.Tasks.Saving.CsvOptions" /&gt; per salvare un progetto come file CSV.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var options = new CsvOptions
{
    DataCategory = DataCategory.Resources,
    TextDelimiter = CsvTextDelimiter.Semicolon,
    Encoding = Encoding.Unicode, IncludeHeaders = true
};

project.Save(OutDir + "WorkWithCsvOptions_out.csv", options);
```

Mostra come utilizzare &lt;see cref="Aspose.Tasks.Saving.CsvOptions" /&gt; per prendere le colonne del diagramma di Gantt predefinito e

```csharp
// salvarle in un file CSV.
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

CsvOptions options = new CsvOptions();
options.TextDelimiter = CsvTextDelimiter.Tab;

var view = project.DefaultView;
options.View = ProjectView.GetDefaultGanttChartView();
options.View.Columns.Clear();

foreach (var t in view.Table.TableFields)
{
    var columnTitle = string.IsNullOrEmpty(t.Title) ? FieldHelper.GetDefaultFieldTitle(t.Field) : t.Title;
    options.View.Columns.Add(new GanttChartColumn(columnTitle, 10, t.Field));
}

project.Save(OutDir + "CustomizeViewForCsvOptions_out.csv", options);
```

### Vedi anche

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


