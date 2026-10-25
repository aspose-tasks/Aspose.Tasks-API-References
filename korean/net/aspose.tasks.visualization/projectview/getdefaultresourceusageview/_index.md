---
title: "ProjectView.GetDefaultResourceUsageView"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectView 메서드. Uid, 이름, 시작, 완료 및 작업 리소스 열을 포함합니다"
type: docs
weight: 50
url: /ko/net/aspose.tasks.visualization/projectview/getdefaultresourceusageview/
---
## ProjectView.GetDefaultResourceUsageView method

Uid, name, start, finish 및 work resource 열을 포함합니다.

```csharp
public static ProjectView GetDefaultResourceUsageView()
```

### 반환 값

`[`ResourceViewColumn`](../../resourceviewcolumn/)` 목록을 포함하는 보기입니다.

## 예제

리소스 사용 보기를 사용하여 프로젝트를 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceUsageView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceUsageView_out.pdf", options);
```

### 또 보기

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


