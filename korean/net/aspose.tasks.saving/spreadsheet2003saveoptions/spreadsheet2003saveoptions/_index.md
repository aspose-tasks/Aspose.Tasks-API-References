---
title: "Spreadsheet2003SaveOptions.Spreadsheet2003SaveOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Spreadsheet2003SaveOptions 생성자. Spreadsheet2003SaveOptions 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.saving/spreadsheet2003saveoptions/spreadsheet2003saveoptions/
---
## Spreadsheet2003SaveOptions constructor

`[`Spreadsheet2003SaveOptions`](../)` 클래스의 새 인스턴스를 초기화합니다.

```csharp
public Spreadsheet2003SaveOptions()
```

## 예제

프로젝트를 Spreadsheet2003 형식으로 내보낼 때 내보낼 열을 추가하는 방법을 보여줍니다.

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

* class [Spreadsheet2003SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../spreadsheet2003saveoptions/)
* assembly [Aspose.Tasks](../../../)


