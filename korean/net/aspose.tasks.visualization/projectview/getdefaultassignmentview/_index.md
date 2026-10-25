---
title: "ProjectView.GetDefaultAssignmentView"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectView 메서드. Uid, 작업 이름, 리소스 이름, 작업량 및 기간 할당 열을 포함합니다"
type: docs
weight: 20
url: /ko/net/aspose.tasks.visualization/projectview/getdefaultassignmentview/
---
## ProjectView.GetDefaultAssignmentView method

Uid, 작업 이름, 리소스 이름, 작업 및 기간 할당 열을 포함합니다.

```csharp
public static ProjectView GetDefaultAssignmentView()
```

### 반환 값

`[`AssignmentViewColumn`](../../assignmentviewcolumn/)` 목록을 포함하는 보기입니다.

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

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


