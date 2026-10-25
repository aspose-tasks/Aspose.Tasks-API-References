---
title: "Klasse CsvOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.CsvOptions klasse. Stelt u in staat om extra opties op te geven bij het opslaan van een project naar CSV."
type: docs
weight: 1980
url: /nl/net/aspose.tasks.saving/csvoptions/
---
## CsvOptions class

Staat toe extra opties op te geven bij het opslaan van een project naar CSV.

```csharp
public class CsvOptions : SimpleSaveOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [CsvOptions](csvoptions/)() | Initialiseert een nieuw exemplaar van de `CsvOptions` klasse die kan worden gebruikt om een project op te slaan in CSV-formaat. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DataCategory](../../aspose.tasks.saving/csvoptions/datacategory/) { get; set; } | Haalt op of stelt een gegevenscategorie in die moet worden opgeslagen. |
| [Encoding](../../aspose.tasks.saving/csvoptions/encoding/) { get; set; } | Haalt op of stelt een codering in waarmee CSV moet worden opgeslagen. |
| [IncludeHeaders](../../aspose.tasks.saving/csvoptions/includeheaders/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of kopteksten al dan niet moeten worden opgenomen (standaardwaarde is TRUE). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Haalt op of stelt het formaat in waarin het document wordt opgeslagen als dit opslaanopties‑object wordt gebruikt. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Haalt op of stelt de comparer in om taken te sorteren op het Gantt‑diagram en het Task‑Sheet‑diagram. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Haalt op of stelt de voorwaarde in die wordt gebruikt om taken te filteren die worden gerenderd op Gantt‑, Task‑Sheet‑ en Task‑Usage‑diagrammen. |
| [TextDelimiter](../../aspose.tasks.saving/csvoptions/textdelimiter/) { get; set; } | Haalt een tekstscheidingsteken op of stelt het in. |
| [View](../../aspose.tasks.saving/csvoptions/view/) { get; set; } | Haalt een lijst op van de weergavekolommen ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) om op te slaan in XLSX-indeling. Indien niet ingesteld, worden de standaardkolommen opgeslagen. |

## Voorbeelden

Toont hoe &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; te gebruiken om een project op te slaan als CSV-bestand.

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


