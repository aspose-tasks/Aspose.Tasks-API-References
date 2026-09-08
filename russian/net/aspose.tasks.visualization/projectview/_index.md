---
title: "Класс ProjectView"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.ProjectView класс. Класс представления проектов"
type: docs
weight: 3300
url: /ru/net/aspose.tasks.visualization/projectview/
---
## ProjectView class

Класс представления проекта

```csharp
public class ProjectView
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ProjectView](projectview/)(IEnumerable&lt;ViewColumn&gt;) | Инициализирует новый экземпляр класса `ProjectView`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Columns](../../aspose.tasks.visualization/projectview/columns/) { get; } | Получает столбцы представления проекта. |

## Методы

| Имя | Описание |
| --- | --- |
| static [GetDefaultAssignmentView](../../aspose.tasks.visualization/projectview/getdefaultassignmentview/)() | Включает столбцы UID, имя задачи, имя ресурса, работу и продолжительность назначения. |
| static [GetDefaultGanttChartView](../../aspose.tasks.visualization/projectview/getdefaultganttchartview/)() | Включает столбцы ID, индикаторы, имя, продолжительность, начало и завершение задачи. |
| static [GetDefaultResourceSheetView](../../aspose.tasks.visualization/projectview/getdefaultresourcesheetview/)() | Включает столбцы UID, имя ресурса, тип, метку материала, инициалы, группу, максимальное количество, стандартную ставку, ставку за сверхурочную работу, стоимость за использование, начисление, базовый календарь и код ресурса. |
| static [GetDefaultResourceUsageView](../../aspose.tasks.visualization/projectview/getdefaultresourceusageview/)() | Включает столбцы Uid, name, start, finish и work resource. |
| static [GetDefaultTaskSheetView](../../aspose.tasks.visualization/projectview/getdefaulttasksheetview/)() | Включает столбцы задачи id, indicators, name, duration, start, finish, predecessors и resource names. |

## Примеры

Показывает, как сохранить проект с представлением назначений.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


