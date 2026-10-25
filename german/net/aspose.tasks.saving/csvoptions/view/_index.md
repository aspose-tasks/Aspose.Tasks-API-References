---
title: "CsvOptions.View"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "CsvOptions-Eigenschaft. Gibt eine Liste der Ansichtsspalten GanttChartColumn zurück oder legt sie fest, die im XLSX‑Format gespeichert werden sollen. Wenn nicht festgelegt, werden die Standardspalten gespeichert."
type: docs
weight: 60
url: /de/net/aspose.tasks.saving/csvoptions/view/
---
## CsvOptions.View property

Gibt eine Liste der Ansichtsspalten ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)) zurück oder legt sie fest, die im XLSX‑Format gespeichert werden sollen. Wenn nicht festgelegt, werden die Standardspalten gespeichert.

```csharp
public ProjectView View { get; set; }
```

## Beispiele

Zeigt, wie man &lt;see cref="Aspose.Tasks.Saving.CsvOptions" /&gt; verwendet, um die Spalten des Standard‑Gantt‑Diagramms zu übernehmen und

```csharp
// sie in einer CSV‑Datei speichert.
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

### Siehe auch

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


