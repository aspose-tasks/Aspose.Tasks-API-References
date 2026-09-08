---
title: "ProjectView.GetDefaultTaskSheetView"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ProjectView. Включает столбцы задачи: id, индикаторы, имя, длительность, начало, завершение, предшественники и имена ресурсов."
type: docs
weight: 60
url: /ru/net/aspose.tasks.visualization/projectview/getdefaulttasksheetview/
---
## ProjectView.GetDefaultTaskSheetView method

Включает столбцы задачи id, indicators, name, duration, start, finish, predecessors и resource names.

```csharp
public static ProjectView GetDefaultTaskSheetView()
```

### Возвращаемое значение

представление, которое содержит список [`GanttChartColumn`](../../ganttchartcolumn/).

## Примеры

Показывает, как сохранить проект с представлением листа задач.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultTaskSheetView()
};

project.Save(OutDir + "WorkWithProjectView_TaskSheetView_out.pdf", options);
```

### См. также

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


