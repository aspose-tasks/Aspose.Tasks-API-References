---
title: "Project.Views"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. View 객체 목록을 가져옵니다"
type: docs
weight: 1020
url: /ko/net/aspose.tasks/project/views/
---
## Project.Views property

[`View`](../../view/) 객체 목록을 가져옵니다.

```csharp
public ViewCollection Views { get; }
```

## 예제

기본 프로젝트 뷰를 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project5.mpp");

View view = null;
foreach (var v in project.Views)
{
    if (v.Name == "&Gantt Chart")
    {
        view = v;
    }
}

// 기본 뷰 설정
project.DefaultView = view;

project.Save(OutDir + @"SaveGantChartView_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### 또 보기

* class [ViewCollection](../../viewcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


