---
title: "Class XlsxOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.XlsxOptions class. Stelt in staat extra opties op te geven bij het renderen van projectpagina's naar XLSX"
type: docs
weight: 2270
url: /nl/net/aspose.tasks.saving/xlsxoptions/
---
## XlsxOptions class

Staat toe extra opties op te geven bij het renderen van projectpagina's naar XLSX.

```csharp
public class XlsxOptions : SimpleSaveOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [XlsxOptions](xlsxoptions/)() | Initialiseert een nieuw exemplaar van de `XlsxOptions`-klasse die kan worden gebruikt om een project op te slaan in XLSX-indeling. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/xlsxoptions/assignmentview/) { get; set; } | Haalt een lijst op of stelt deze in van de weergavekolommen voor toewijzingen die moeten worden gerenderd ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [Encoding](../../aspose.tasks.saving/xlsxoptions/encoding/) { get; set; } | Haalt de codering van het resulterende XLSX-bestand op of stelt deze in. De standaardwaarde is UTF8. |
| [ResourceView](../../aspose.tasks.saving/xlsxoptions/resourceview/) { get; set; } | Haalt een lijst op of stelt deze in van de weergavekolommen voor resources die moeten worden gerenderd ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Haalt op of stelt het formaat in waarin het document wordt opgeslagen als dit opslaanopties‑object wordt gebruikt. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Haalt op of stelt de comparer in om taken te sorteren op het Gantt‑diagram en het Task‑Sheet‑diagram. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Haalt op of stelt de voorwaarde in die wordt gebruikt om taken te filteren die worden gerenderd op Gantt‑, Task‑Sheet‑ en Task‑Usage‑diagrammen. |
| [View](../../aspose.tasks.saving/xlsxoptions/view/) { get; set; } | Haalt een lijst op van de weergavekolommen ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) om op te slaan in XLSX-indeling. Indien niet ingesteld, worden de standaardkolommen opgeslagen. |

## Voorbeelden

Toont hoe een project op te slaan in een XLSX-bestand door gebruik te maken van &lt;see cref="P:Aspose.Tasks.Saving.XlsxOptions"&gt;Days&lt;/see&gt; opties.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new XlsxOptions();

// Voeg gewenste Gantt Chart kolommen toe
var col = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(col);

// Voeg gewenste resource view kolommen toe
var rscCol = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(rscCol);

// Voeg gewenste assignment view kolommen toe
var assnCol = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assnCol);

// stel codering in
options.Encoding = Encoding.Unicode;

project.Save(OutDir + "UsingXlsxOptions_out.xlsx", options);
```

### Zie ook

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


