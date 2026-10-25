---
title: "CsvOptions.View"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CsvOptions-eigenschap. Haalt op of stelt een lijst van de weergavekolommen GanttChartColumn in om op te slaan in XLSX-formaat. Indien niet ingesteld, worden de standaardkolommen opgeslagen"
type: docs
weight: 60
url: /nl/net/aspose.tasks.saving/csvoptions/view/
---
## CsvOptions.View property

Haalt op of stelt een lijst van de weergavekolommen ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)) in om op te slaan in XLSX-formaat. Indien niet ingesteld, worden de standaardkolommen opgeslagen.

```csharp
public ProjectView View { get; set; }
```

## Voorbeelden

Toont hoe &lt;see cref="Aspose.Tasks.Saving.CsvOptions" /&gt; te gebruiken om de kolommen van de standaard Gantt-diagram te nemen en

```csharp
// sla ze op in een CSV-bestand.
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

### Zie ook

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


