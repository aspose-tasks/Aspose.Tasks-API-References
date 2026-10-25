---
title: "ProjectView.GetDefaultTaskSheetView"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectView 메서드. id, 지시자, 이름, 기간, 시작, 완료, 선행 작업 및 리소스 이름 작업 열을 포함합니다"
type: docs
weight: 60
url: /ko/net/aspose.tasks.visualization/projectview/getdefaulttasksheetview/
---
## ProjectView.GetDefaultTaskSheetView method

id, indicators, name, duration, start, finish, predecessors 및 resource names 작업 열을 포함합니다.

```csharp
public static ProjectView GetDefaultTaskSheetView()
```

### 반환 값

[`GanttChartColumn`](../../ganttchartcolumn/) 목록을 포함하는 보기입니다.

## 예제

작업 시트 보기를 사용하여 프로젝트를 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultTaskSheetView()
};

project.Save(OutDir + "WorkWithProjectView_TaskSheetView_out.pdf", options);
```

### 또 보기

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


