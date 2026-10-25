---
title: "ProjectView.ProjectView"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор ProjectView. Инициализирует новый экземпляр класса ProjectView."
type: docs
weight: 10
url: /ru/net/aspose.tasks.visualization/projectview/projectview/
---
## ProjectView constructor

Инициализирует новый экземпляр класса [`ProjectView`](../).

```csharp
public ProjectView(IEnumerable<ViewColumn> columns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| столбцы | IEnumerable`1 | Список столбцов представления. |

## Примеры

Показывает, как сохранить проект с представлением, содержащим пользовательский набор столбцов.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new GanttChartColumn("Name", 100, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("Finish", 100, Field.TaskFinish),
    new GanttChartColumn("Cost2", 80, Field.TaskCost2),
    new GanttChartColumn("Number6", 80, Field.TaskNumber6),
    new GanttChartColumn("Date6", 80, Field.TaskDate6),
    new GanttChartColumn("Flag6", 80, Field.TaskFlag6),
    new GanttChartColumn("Flag18", 80, Field.TaskFlag18),
    new GanttChartColumn("Duration6", 80, Field.TaskDuration6)
};
options.View = new ProjectView(columns);

// перебрать столбцы представления
foreach (var column in options.View.Columns)
{
    Console.WriteLine("Column Name: " + column.Name);
}

options.PresentationFormat = PresentationFormat.TaskUsage;
project.Save(OutDir + "TaskUsageProjectView_Columns.pdf", options);
```

### См. также

* class [ViewColumn](../../viewcolumn/)
* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


