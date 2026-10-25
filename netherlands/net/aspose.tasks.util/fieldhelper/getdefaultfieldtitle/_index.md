---
title: "FieldHelper.GetDefaultFieldTitle"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "FieldHelper-methode. Retourneert een standaardtitel van het specifieke veld"
type: docs
weight: 10
url: /nl/net/aspose.tasks.util/fieldhelper/getdefaultfieldtitle/
---
## FieldHelper.GetDefaultFieldTitle method

Retourneert een standaardtitel van het specifieke veld.

```csharp
public static string GetDefaultFieldTitle(Field field)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| veld | Veld | Veld om een standaardtitel te verkrijgen. |

### Retourwaarde

Een standaardtitel van het specifieke veld als het veld kan worden weergegeven in de weergave van MS Project, anders null.

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

* enum [Field](../../../aspose.tasks/field/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


