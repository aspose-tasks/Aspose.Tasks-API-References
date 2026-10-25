---
title: "클래스 Spreadsheet2003SaveOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.Spreadsheet2003SaveOptions 클래스. 프로젝트 페이지를 Spreadsheet2003으로 렌더링할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 2220
url: /ko/net/aspose.tasks.saving/spreadsheet2003saveoptions/
---
## Spreadsheet2003SaveOptions class

프로젝트 페이지를 Spreadsheet2003으로 렌더링할 때 추가 옵션을 지정할 수 있습니다.

```csharp
public class Spreadsheet2003SaveOptions : SimpleSaveOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Spreadsheet2003SaveOptions](spreadsheet2003saveoptions/)() | 새 `Spreadsheet2003SaveOptions` 클래스 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/spreadsheet2003saveoptions/assignmentview/) { get; set; } | 렌더링할 할당 보기 열 목록을 가져오거나 설정합니다 ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [ResourceView](../../aspose.tasks.saving/spreadsheet2003saveoptions/resourceview/) { get; set; } | 렌더링할 리소스 보기 열 목록을 가져오거나 설정합니다 ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 이 저장 옵션 개체가 사용될 경우 문서가 저장되는 형식을 가져오거나 설정합니다. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 간트 차트 및 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 가져오거나 설정합니다. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 간트, 작업 시트 및 작업 사용 차트에 렌더링된 작업을 필터링하는 데 사용되는 조건을 가져오거나 설정합니다. |
| [View](../../aspose.tasks.saving/spreadsheet2003saveoptions/view/) { get; set; } | 저장할 보기 열 목록을 가져오거나 설정합니다 ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). 설정하지 않으면 기본 열이 저장됩니다. |

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


