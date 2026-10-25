---
title: "Project.DefaultView"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. 프로젝트의 기본 뷰를 가져오거나 설정합니다"
type: docs
weight: 360
url: /ko/net/aspose.tasks/project/defaultview/
---
## Project.DefaultView property

프로젝트의 기본 보기를 가져오거나 설정합니다.

```csharp
public View DefaultView { get; set; }
```

## 예제

프로젝트의 기본 뷰를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// 기본 뷰 가져오기
UsageView view = (TaskUsageView)project.DefaultView;

// 세부 정보 헤더 열이 표시되지 않습니다
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// 세부 정보 헤더 열 표시
view.DisplayDetailsHeaderColumn = true;

// 모든 할당 행에 세부 정보 헤더 반복
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

Project의 뷰를 작업하고 기본 뷰에 열을 추가하는 방법을 보여줍니다(이는 MPP 파일을 MS Project에서 열었을 때 표시되는 뷰입니다).

```csharp
// 뷰 없이 빈 프로젝트를 생성합니다.
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// 기본 뷰를 수정합니다(이 뷰는 간트 차트 뷰입니다).
// 또는 project.View 컬렉션을 사용하여 이름이나 View Screen으로 뷰를 선택할 수 있습니다.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// WriteViewData 플래그는 뷰 속성의 수정 사항을 영구히 저장하는 데 사용해야 합니다.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

### 또 보기

* class [View](../../view/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


