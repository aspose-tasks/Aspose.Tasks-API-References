---
title: "ProjectView.GetDefaultResourceSheetView"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectView 메서드. Uid, 리소스 이름, 유형, 재료, 라벨, 이니셜, 그룹, 최대 단위, 표준 요율, 초과 근무 요율, 사용당 비용, 기본 달력에서 발생 및 코드 리소스 열을 포함합니다"
type: docs
weight: 40
url: /ko/net/aspose.tasks.visualization/projectview/getdefaultresourcesheetview/
---
## ProjectView.GetDefaultResourceSheetView method

Uid, 리소스 이름, 유형, 재료 라벨, 이니셜, 그룹, 최대 단위, 표준 요금, 초과 근무 요금, 사용당 비용, 발생 시점, 기본 캘린더 및 코드 리소스 열을 포함합니다.

```csharp
public static ProjectView GetDefaultResourceSheetView()
```

### 반환 값

`[`ResourceViewColumn`](../../resourceviewcolumn/)` 목록을 포함하는 보기입니다.

## 예제

리소스 시트 보기를 사용하여 프로젝트를 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceSheetView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceSheetView_out.pdf", options);
```

### 또 보기

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


