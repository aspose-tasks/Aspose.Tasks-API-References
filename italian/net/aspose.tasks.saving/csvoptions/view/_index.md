---
title: "CsvOptions.View"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà CsvOptions. Ottiene o imposta un elenco delle colonne di visualizzazione GanttChartColumn da salvare nel formato XLSX. Se non impostato, vengono salvate le colonne predefinite"
type: docs
weight: 60
url: /it/net/aspose.tasks.saving/csvoptions/view/
---
## CsvOptions.View property

Ottiene o imposta un elenco delle colonne di visualizzazione ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)) da salvare nel formato XLSX. Se non impostato, vengono salvate le colonne predefinite.

```csharp
public ProjectView View { get; set; }
```

## Esempi

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

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


