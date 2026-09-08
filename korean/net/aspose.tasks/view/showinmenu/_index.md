---
title: "View.ShowInMenu"
second_title: "Aspose.Tasks for .NET API 참조"
description: "View 속성. Microsoft Project가 리본의 View 또는 Other Views 드롭다운 목록에 단일 보기 이름을 표시하는지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 90
url: /ko/net/aspose.tasks/view/showinmenu/
---
## View.ShowInMenu property

Microsoft Project가 리본의 보기 또는 기타 보기 드롭다운 목록에 단일 보기 이름을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool ShowInMenu { get; set; }
```

## 예제

MS Project 뷰 작업 방법을 보여줍니다.

```csharp
// 뷰 없이 빈 프로젝트를 생성합니다.
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// 표준 간트 차트 뷰를 생성합니다.
View view = new GanttChartView();

// 몇 가지 뷰 속성을 설정합니다.
// Microsoft Project가 리본의 View 또는 Other Views 드롭다운 목록에 단일 뷰 이름을 표시할지 여부를 나타내는 값을 설정합니다.
view.ShowInMenu = true;
// Microsoft Project가 단일 뷰에 대한 필터를 강조 표시할지 여부를 나타내는 값을 설정합니다.
view.HighlightFilter = true;

// 다음 속성의 쓰기는 지원되지 않습니다.
// 단일 뷰에서 사용되는 필터를 설정합니다.
view.Filter = null;
// 단일 뷰의 그룹을 설정합니다.
view.Group = null;
// 단일 뷰의 테이블을 설정합니다.
view.Table = null;

// 몇 가지 뷰 설정을 조정합니다.
// 모든 페이지에 인쇄될 첫 번째 열의 개수를 설정합니다.
view.PageInfo.PageViewSettings.FirstColumnsCount = 4;
// 모든 페이지에 지정된 수의 첫 번째 열을 인쇄할지 여부를 나타내는 값을 설정합니다.
view.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

// 우리 프로젝트에 뷰를 추가합니다.
project.Views.Add(view);

// WriteViewData 플래그는 project.Views의 수정 사항을 지속하는 데 사용되어야 합니다.
project.Save(OutDir + "WorkWithView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
// 새로 추가된 뷰의 몇 가지 속성을 확인합니다.
// 뷰의 고유 식별자를 출력합니다.
Console.WriteLine("View Uid: " + view.Uid);
// 단일 뷰의 화면 유형을 출력합니다.
Console.WriteLine("View Screen: " + view.Screen);
Console.WriteLine("View Type: " + view.Type);
Console.WriteLine("Parent Project of the view: " + view.ParentProject.Get(Prj.Name));
```

### 또 보기

* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


