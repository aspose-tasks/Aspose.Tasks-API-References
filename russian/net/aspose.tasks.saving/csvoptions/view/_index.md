---
title: "CsvOptions.View"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство CsvOptions. Получает или задает список столбцов представления GanttChartColumn для сохранения в формате XLSX. Если не задано, сохраняются столбцы по умолчанию"
type: docs
weight: 60
url: /ru/net/aspose.tasks.saving/csvoptions/view/
---
## CsvOptions.View property

Получает или задает список столбцов представления ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)) для сохранения в формате XLSX. Если не задано, сохраняются столбцы по умолчанию.

```csharp
public ProjectView View { get; set; }
```

## Примеры

Показывает, как использовать &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; для получения столбцов диаграммы Ганта по умолчанию и

```csharp
// сохранить их в файл CSV.
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

### См. также

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


