---
title: "XlsxOptions.Encoding"
second_title: "Aspose.Tasks for .NET API 참조"
description: "XlsxOptions 속성. 결과 XLSX 파일의 인코딩을 가져오거나 설정합니다. 기본값은 UTF8입니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.saving/xlsxoptions/encoding/
---
## XlsxOptions.Encoding property

결과 XLSX 파일의 인코딩을 가져오거나 설정합니다. 기본값은 UTF8입니다.

```csharp
public Encoding Encoding { get; set; }
```

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

* class [XlsxOptions](../)
* namespace [Aspose.Tasks.Saving](../../xlsxoptions/)
* assembly [Aspose.Tasks](../../../)


