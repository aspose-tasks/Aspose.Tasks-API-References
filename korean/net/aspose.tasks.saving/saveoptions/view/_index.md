---
title: "SaveOptions.View"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 렌더링할 view 열 목록(GanttChartColumn)을 가져오거나 설정합니다. 설정하지 않으면 작업 ID, 작업 이름, 시작 및 종료만 렌더링됩니다. View와 ViewSettings 속성이 모두 설정된 경우, View의 열이 ViewSettings의 열을 우선합니다."
type: docs
weight: 230
url: /ko/net/aspose.tasks.saving/saveoptions/view/
---
## SaveOptions.View property

렌더링할 view 열 목록([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/))을 가져오거나 설정합니다. 설정하지 않으면 작업 ID, 작업 이름, 시작 및 종료만 렌더링됩니다. View와 [`ViewSettings`](../viewsettings/) 속성이 모두 설정된 경우, View의 열이 ViewSettings의 열을 우선합니다.

```csharp
public ProjectView View { get; set; }
```

## 예제

프로젝트를 내보낼 때 내보낼 view 열을 추가하는 방법을 보여줍니다.

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

### 또 보기

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


