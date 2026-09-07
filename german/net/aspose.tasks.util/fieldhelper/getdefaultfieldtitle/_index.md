---
title: "FieldHelper.GetDefaultFieldTitle"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "FieldHelper-Methode. Gibt einen Standardtitel des jeweiligen Feldes zurück"
type: docs
weight: 10
url: /de/net/aspose.tasks.util/fieldhelper/getdefaultfieldtitle/
---
## FieldHelper.GetDefaultFieldTitle method

Gibt einen Standardtitel des jeweiligen Feldes zurück.

```csharp
public static string GetDefaultFieldTitle(Field field)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Feld | Feld | Feld, um einen Standardtitel zu erhalten. |

### Rückgabewert

Ein Standardtitel des jeweiligen Feldes, wenn das Feld in der Ansicht von MS Project angezeigt werden kann, andernfalls null.

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

* enum [Field](../../../aspose.tasks/field/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


