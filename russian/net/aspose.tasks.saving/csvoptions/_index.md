---
title: "Класс CsvOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Saving.CsvOptions. Позволяет задавать дополнительные параметры при сохранении проекта в CSV"
type: docs
weight: 1980
url: /ru/net/aspose.tasks.saving/csvoptions/
---
## CsvOptions class

Позволяет указать дополнительные параметры при сохранении проекта в CSV.

```csharp
public class CsvOptions : SimpleSaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CsvOptions](csvoptions/)() | Инициализирует новый экземпляр класса `CsvOptions`, который можно использовать для сохранения проекта в формате CSV. |

## Свойства

| Имя | Описание |
| --- | --- |
| [DataCategory](../../aspose.tasks.saving/csvoptions/datacategory/) { get; set; } | Получает или задает категорию данных для сохранения. |
| [Encoding](../../aspose.tasks.saving/csvoptions/encoding/) { get; set; } | Получает или задает кодировку, с которой сохраняется CSV. |
| [IncludeHeaders](../../aspose.tasks.saving/csvoptions/includeheaders/) { get; set; } | Получает или задает значение, указывающее, включать ли заголовки (значение по умолчанию — TRUE). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Получает или задает формат, в котором будет сохраняться документ, если используется этот объект параметров сохранения. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Получает или задает компаратор для сортировки задач на диаграмме Ганта и листе задач. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Получает или задает условие, используемое для фильтрации задач, отрисованных на диаграммах Ганта, листе задач и использовании задач. |
| [TextDelimiter](../../aspose.tasks.saving/csvoptions/textdelimiter/) { get; set; } | Получает или задает разделитель текста. |
| [View](../../aspose.tasks.saving/csvoptions/view/) { get; set; } | Получает или задает список столбцов представления ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)), которые сохраняются в формате XLSX. Если не задано, сохраняются столбцы по умолчанию. |

## Примеры

Показывает, как использовать &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; для сохранения проекта в виде CSV-файла.

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


