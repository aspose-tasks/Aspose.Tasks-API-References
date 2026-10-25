---
title: "클래스 ProjectView"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.ProjectView 클래스. 프로젝트 뷰 클래스"
type: docs
weight: 3300
url: /ko/net/aspose.tasks.visualization/projectview/
---
## ProjectView class

프로젝트 보기 클래스

```csharp
public class ProjectView
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ProjectView](projectview/)(IEnumerable&lt;ViewColumn&gt;) | `ProjectView` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Columns](../../aspose.tasks.visualization/projectview/columns/) { get; } | 프로젝트 뷰 열을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| static [GetDefaultAssignmentView](../../aspose.tasks.visualization/projectview/getdefaultassignmentview/)() | Uid, 작업 이름, 리소스 이름, 작업 및 기간 할당 열을 포함합니다. |
| static [GetDefaultGanttChartView](../../aspose.tasks.visualization/projectview/getdefaultganttchartview/)() | id, 표시기, 이름, 기간, 시작 및 종료 작업 열을 포함합니다. |
| static [GetDefaultResourceSheetView](../../aspose.tasks.visualization/projectview/getdefaultresourcesheetview/)() | Uid, 리소스 이름, 유형, 재료 라벨, 이니셜, 그룹, 최대 단위, 표준 요금, 초과 근무 요금, 사용당 비용, 발생 시점, 기본 캘린더 및 코드 리소스 열을 포함합니다. |
| static [GetDefaultResourceUsageView](../../aspose.tasks.visualization/projectview/getdefaultresourceusageview/)() | Uid, name, start, finish 및 work resource 열을 포함합니다. |
| static [GetDefaultTaskSheetView](../../aspose.tasks.visualization/projectview/getdefaulttasksheetview/)() | id, indicators, name, duration, start, finish, predecessors 및 resource names 작업 열을 포함합니다. |

## 예제

assignment view를 사용하여 프로젝트를 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### 또 보기

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


