---
title: "FieldHelper.GetDefaultFieldTitle"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод FieldHelper. Возвращает заголовок по умолчанию конкретного поля."
type: docs
weight: 10
url: /ru/net/aspose.tasks.util/fieldhelper/getdefaultfieldtitle/
---
## FieldHelper.GetDefaultFieldTitle method

Возвращает заголовок по умолчанию для конкретного поля.

```csharp
public static string GetDefaultFieldTitle(Field field)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поле | Поле | Поле для получения заголовка по умолчанию. |

### Возвращаемое значение

Заголовок по умолчанию конкретного поля, если поле может быть отображено в представлении MS Project, иначе null.

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

* enum [Field](../../../aspose.tasks/field/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


