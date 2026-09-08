---
title: "클래스 ResourceUsageView"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ResourceUsageView 클래스. 프로젝트에서 리소스 사용 보기를 나타냅니다"
type: docs
weight: 1810
url: /ko/net/aspose.tasks/resourceusageview/
---
## ResourceUsageView class

프로젝트 내 리소스 사용 보기를 나타냅니다.

```csharp
public sealed class ResourceUsageView : UsageView
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [AlignDetailsData](../../aspose.tasks/usageview/aligndetailsdata/) { get; set; } | 세부 데이터 정렬을 가져오거나 설정합니다. |
| [BottomTimescaleTier](../../aspose.tasks/usageview/bottomtimescaletier/) { get; set; } | 뷰 하단 타임스케일 티어의 설정을 가져오거나 설정합니다. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [DisplayDetailsHeaderColumn](../../aspose.tasks/usageview/displaydetailsheadercolumn/) { get; set; } | 뷰에 세부 헤더 열을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [DisplayShortDetailHeaderNames](../../aspose.tasks/usageview/displayshortdetailheadernames/) { get; set; } | 짧은 상세 헤더 이름을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [FieldCollection](../../aspose.tasks/resourceusageview/fieldcollection/) { get; } | 이 ResourceUsageView의 [`ResourceUsageViewFieldCollection`](../resourceusageviewfieldcollection/) 객체를 가져옵니다. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | 단일 보기에서 사용되는 필터를 가져오거나 설정합니다. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | 단일 보기의 그룹을 가져오거나 설정합니다. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Microsoft Project가 단일 보기의 필터를 강조 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [MiddleTimescaleTier](../../aspose.tasks/usageview/middletimescaletier/) { get; set; } | 보기의 중간 시간축 단계 설정을 가져오거나 설정합니다. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Name](../../aspose.tasks/view/name/) { get; set; } | View 객체의 이름을 가져오거나 설정합니다. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | [`PageInfo`](../view/pageinfo/) 클래스의 인스턴스를 가져옵니다. mpp 파일 형식에 존재하는 페이지 설정 데이터를 나타냅니다. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | View 객체의 상위 항목을 가져옵니다. 읽기 전용 [`Project`](../project/). |
| [RepeatDetailsHeaderOnAllRows](../../aspose.tasks/usageview/repeatdetailsheaderonallrows/) { get; set; } | 모든 할당 행에 상세 헤더를 반복할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Screen](../../aspose.tasks/view/screen/) { get; } | 단일 보기의 화면 유형을 가져옵니다. 읽기 전용 [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Microsoft Project가 리본의 보기 또는 기타 보기 드롭다운 목록에 단일 보기 이름을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | 단일 보기의 테이블을 가져오거나 설정합니다. |
| [TimescaleSizePercentage](../../aspose.tasks/usageview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/usageview/toptimescaletier/) { get; set; } | 보기의 상단 시간축 단계 설정을 가져오거나 설정합니다. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Type](../../aspose.tasks/view/type/) { get; } | 단일 보기의 항목 유형(예: 작업 또는 리소스)을 가져옵니다. 읽기 전용 [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | 보기의 고유 식별자를 가져옵니다. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | 보기에서 [`OleObject`](../oleobject/)의 배치 및 모양을 나타내는 객체 컬렉션을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | 현재 인스턴스를 동일한 유형의 다른 객체와 비교하고, 현재 인스턴스가 정렬 순서에서 앞선, 뒤에 있거나 같은 위치에 있는지를 나타내는 정수를 반환합니다. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | [`Resource`](../resource/) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다. |

## 예제

리소스 사용 보기를 렌더링하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

// 필요한 TimeScale 설정을 Days로 지정하여 SaveOptions를 정의합니다.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Days,

    // Presentation 형식을 ResourceUsage로 설정합니다.
    PresentationFormat = PresentationFormat.ResourceUsage
};

project.Save(OutDir + "ResourceUsage_days_out.pdf", options);
```

### 또 보기

* class [UsageView](../usageview/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


