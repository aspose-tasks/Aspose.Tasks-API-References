---
title: "SaveOptions.View"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает список столбцов представления для рендеринга GanttChartColumn. Если не задано, отображаются только идентификаторы задач, их имена, начало и окончание. Если заданы оба свойства View и ViewSettings, столбцы из View переопределяют столбцы из ViewSettings."
type: docs
weight: 230
url: /ru/net/aspose.tasks.saving/saveoptions/view/
---
## SaveOptions.View property

Получает или задает список столбцов представления для рендеринга ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)). Если не задано, отображаются только идентификаторы задач, их имена, начало и окончание. Если заданы оба свойства View и [`ViewSettings`](../viewsettings/), столбцы из View переопределяют столбцы из ViewSettings.

```csharp
public ProjectView View { get; set; }
```

## Примеры

Показано, как добавить столбцы представления для экспорта при экспорте проекта.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();
var ganttChartColumn = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(ganttChartColumn);

var resourceViewColumn = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(resourceViewColumn);

var assignmentViewColumn = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assignmentViewColumn);

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### См. также

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


