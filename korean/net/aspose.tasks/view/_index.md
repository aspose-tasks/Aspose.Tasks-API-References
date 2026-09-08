---
title: "클래스 View"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.View 클래스. Project에서 뷰를 나타냅니다."
type: docs
weight: 2890
url: /ko/net/aspose.tasks/view/
---
## View class

Project의 뷰를 나타냅니다.

```csharp
public class View : IComparable<View>
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [View](view/#constructor)() | 새 `View` 클래스 인스턴스를 초기화합니다. |
| [View](view/#constructor_1)(ViewScreen) | 새 `View` 클래스 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | 단일 보기에서 사용되는 필터를 가져오거나 설정합니다. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | 단일 보기의 그룹을 가져오거나 설정합니다. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Microsoft Project가 단일 보기의 필터를 강조 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | View 객체의 이름을 가져오거나 설정합니다. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | [`PageInfo`](./pageinfo/) 클래스의 인스턴스를 가져옵니다. mpp 파일 형식에 존재하는 페이지 설정 데이터를 나타냅니다. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | View 객체의 상위 항목을 가져옵니다. 읽기 전용 [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | 단일 보기의 화면 유형을 가져옵니다. 읽기 전용 [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Microsoft Project가 리본의 보기 또는 기타 보기 드롭다운 목록에 단일 보기 이름을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | 단일 보기의 테이블을 가져오거나 설정합니다. |
| [Type](../../aspose.tasks/view/type/) { get; } | 단일 보기의 항목 유형(예: 작업 또는 리소스)을 가져옵니다. 읽기 전용 [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | 보기의 고유 식별자를 가져옵니다. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | 보기에서 [`OleObject`](../oleobject/)의 배치 및 모양을 나타내는 객체 컬렉션을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | 현재 인스턴스를 동일한 유형의 다른 객체와 비교하고, 현재 인스턴스가 정렬 순서에서 앞선, 뒤에 있거나 같은 위치에 있는지를 나타내는 정수를 반환합니다. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | [`Resource`](../resource/) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다. |
| [operator ==](../../aspose.tasks/view/op_equality/) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [operator &gt;](../../aspose.tasks/view/op_greaterthan/) | 이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값을 반환합니다. |
| [operator &gt;=](../../aspose.tasks/view/op_greaterthanorequal/) | 이 인스턴스가 지정된 객체보다 크거나 같은지 여부를 나타내는 값을 반환합니다. |
| [operator !=](../../aspose.tasks/view/op_inequality/) | 이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값을 반환합니다. |
| [operator &lt;](../../aspose.tasks/view/op_lessthan/) | 이 인스턴스가 지정된 객체보다 작은지 여부를 나타내는 값을 반환합니다. |
| [operator &lt;=](../../aspose.tasks/view/op_lessthanorequal/) | 이 인스턴스가 지정된 객체보다 작거나 같은지 여부를 나타내는 값을 반환합니다. |

## 예제

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


