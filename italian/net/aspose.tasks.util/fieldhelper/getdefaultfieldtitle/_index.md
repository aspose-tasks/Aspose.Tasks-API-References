---
title: "FieldHelper.GetDefaultFieldTitle"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo FieldHelper. Restituisce un titolo predefinito del campo specifico"
type: docs
weight: 10
url: /it/net/aspose.tasks.util/fieldhelper/getdefaultfieldtitle/
---
## FieldHelper.GetDefaultFieldTitle method

Restituisce un titolo predefinito del campo specifico.

```csharp
public static string GetDefaultFieldTitle(Field field)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| campo | Campo | Campo per ottenere un titolo predefinito. |

### Valore di ritorno

Un titolo predefinito del campo specifico se il campo può essere visualizzato nella vista di MS Project, altrimenti null.

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

* enum [Field](../../../aspose.tasks/field/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


