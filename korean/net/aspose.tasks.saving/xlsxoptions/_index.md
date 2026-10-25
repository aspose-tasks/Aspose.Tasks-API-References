---
title: "클래스 XlsxOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.XlsxOptions 클래스. 프로젝트 페이지를 XLSX로 렌더링할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 2270
url: /ko/net/aspose.tasks.saving/xlsxoptions/
---
## XlsxOptions class

프로젝트 페이지를 XLSX로 렌더링할 때 추가 옵션을 지정할 수 있습니다.

```csharp
public class XlsxOptions : SimpleSaveOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [XlsxOptions](xlsxoptions/)() | `XlsxOptions` 클래스의 새 인스턴스를 초기화합니다. 이 인스턴스를 사용하여 프로젝트를 XLSX 형식으로 저장할 수 있습니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/xlsxoptions/assignmentview/) { get; set; } | 렌더링할 할당 보기 열 목록을 가져오거나 설정합니다 ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [Encoding](../../aspose.tasks.saving/xlsxoptions/encoding/) { get; set; } | 결과 XLSX 파일의 인코딩을 가져오거나 설정합니다. 기본값은 UTF8입니다. |
| [ResourceView](../../aspose.tasks.saving/xlsxoptions/resourceview/) { get; set; } | 렌더링할 리소스 보기 열 목록을 가져오거나 설정합니다 ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 이 저장 옵션 개체가 사용될 경우 문서가 저장되는 형식을 가져오거나 설정합니다. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 간트 차트 및 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 가져오거나 설정합니다. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 간트, 작업 시트 및 작업 사용 차트에 렌더링된 작업을 필터링하는 데 사용되는 조건을 가져오거나 설정합니다. |
| [View](../../aspose.tasks.saving/xlsxoptions/view/) { get; set; } | XLSX 형식으로 저장할 보기 열 목록([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/))을 가져오거나 설정합니다. 설정하지 않으면 기본 열이 저장됩니다. |

## 예제

&lt;see cref=\"P:Aspose.Tasks.Saving.XlsxOptions\"&gt;Days&lt;/see&gt; 옵션을 사용하여 프로젝트를 XLSX 파일로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new XlsxOptions();

// 원하는 Gantt 차트 열 추가
var col = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(col);

// 원하는 리소스 보기 열 추가
var rscCol = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(rscCol);

// 원하는 할당 보기 열 추가
var assnCol = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assnCol);

// 인코딩 설정
options.Encoding = Encoding.Unicode;

project.Save(OutDir + "UsingXlsxOptions_out.xlsx", options);
```

### 또 보기

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


