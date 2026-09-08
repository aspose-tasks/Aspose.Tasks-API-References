---
title: "Класс XlsxOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Saving.XlsxOptions. Позволяет задавать дополнительные параметры при рендеринге страниц проекта в XLSX."
type: docs
weight: 2270
url: /ru/net/aspose.tasks.saving/xlsxoptions/
---
## XlsxOptions class

Позволяет указать дополнительные параметры при рендеринге страниц проекта в XLSX.

```csharp
public class XlsxOptions : SimpleSaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [XlsxOptions](xlsxoptions/)() | Инициализирует новый экземпляр класса `XlsxOptions`, который можно использовать для сохранения проекта в формате XLSX. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/xlsxoptions/assignmentview/) { get; set; } | Получает или задает список столбцов представления назначений для отображения ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [Encoding](../../aspose.tasks.saving/xlsxoptions/encoding/) { get; set; } | Получает или задает кодировку результирующего файла XLSX. Значение по умолчанию — UTF8. |
| [ResourceView](../../aspose.tasks.saving/xlsxoptions/resourceview/) { get; set; } | Получает или задает список столбцов представления ресурсов для отображения ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Получает или задает формат, в котором будет сохраняться документ, если используется этот объект параметров сохранения. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Получает или задает компаратор для сортировки задач на диаграмме Ганта и листе задач. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Получает или задает условие, используемое для фильтрации задач, отрисованных на диаграммах Ганта, листе задач и использовании задач. |
| [View](../../aspose.tasks.saving/xlsxoptions/view/) { get; set; } | Получает или задает список столбцов представления ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)), которые сохраняются в формате XLSX. Если не задано, сохраняются столбцы по умолчанию. |

## Примеры

Показывает, как сохранить проект в файл XLSX, используя параметры &lt;see cref=\"P:Aspose.Tasks.Saving.XlsxOptions\"&gt;Days&lt;/see&gt;.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new XlsxOptions();

// Добавьте нужные столбцы диаграммы Ганта
var col = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(col);

// Добавьте нужные столбцы представления ресурсов
var rscCol = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(rscCol);

// Добавьте нужные столбцы представления назначений
var assnCol = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assnCol);

// установить кодировку
options.Encoding = Encoding.Unicode;

project.Save(OutDir + "UsingXlsxOptions_out.xlsx", options);
```

### См. также

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


