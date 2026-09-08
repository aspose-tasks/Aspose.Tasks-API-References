---
title: "ProjectView.GetDefaultAssignmentView"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ProjectView. Включает столбцы назначения Uid, task, name, resource, name, work и duration"
type: docs
weight: 20
url: /ru/net/aspose.tasks.visualization/projectview/getdefaultassignmentview/
---
## ProjectView.GetDefaultAssignmentView method

Включает столбцы UID, имя задачи, имя ресурса, работу и продолжительность назначения.

```csharp
public static ProjectView GetDefaultAssignmentView()
```

### Возвращаемое значение

представление, которое содержит список [`AssignmentViewColumn`](../../assignmentviewcolumn/).

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

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


