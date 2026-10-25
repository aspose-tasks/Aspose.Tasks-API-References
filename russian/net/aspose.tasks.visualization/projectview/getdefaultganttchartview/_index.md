---
title: "ProjectView.GetDefaultGanttChartView"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ProjectView. Включает столбцы задачи: id, индикаторы, имя, длительность, начало и завершение"
type: docs
weight: 30
url: /ru/net/aspose.tasks.visualization/projectview/getdefaultganttchartview/
---
## ProjectView.GetDefaultGanttChartView method

Включает столбцы ID, индикаторы, имя, продолжительность, начало и завершение задачи.

```csharp
public static ProjectView GetDefaultGanttChartView()
```

### Возвращаемое значение

представление, которое содержит список [`GanttChartColumn`](../../ganttchartcolumn/).

## Примеры

Показывает, как сохранить проект с представлением диаграммы Ганта.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultGanttChartView()
};

project.Save(OutDir + "WorkWithProjectView_GanttChartView_out.pdf", options);
```

### См. также

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


