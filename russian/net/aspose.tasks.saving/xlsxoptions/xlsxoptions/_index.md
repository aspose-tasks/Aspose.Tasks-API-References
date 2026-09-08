---
title: "XlsxOptions.XlsxOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор XlsxOptions. Инициализирует новый экземпляр класса XlsxOptions, который можно использовать для сохранения проекта в формате XLSX."
type: docs
weight: 10
url: /ru/net/aspose.tasks.saving/xlsxoptions/xlsxoptions/
---
## XlsxOptions constructor

Инициализирует новый экземпляр класса [`XlsxOptions`](../), который можно использовать для сохранения проекта в формате XLSX.

```csharp
public XlsxOptions()
```

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

* class [XlsxOptions](../)
* namespace [Aspose.Tasks.Saving](../../xlsxoptions/)
* assembly [Aspose.Tasks](../../../)


