---
title: "UsageView.DisplayDetailsHeaderColumn"
second_title: "Aspose.Tasks for .NET API 참조"
description: "UsageView 속성. 보기에서 상세 헤더 열을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/usageview/displaydetailsheadercolumn/
---
## UsageView.DisplayDetailsHeaderColumn property

뷰에 세부 헤더 열을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool DisplayDetailsHeaderColumn { get; set; }
```

## 예제

작업 사용 보기와 상세 정보를 렌더링하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// 보기를 가져옵니다
UsageView view = (TaskUsageView)project.DefaultView;

// 상세 헤더 열이 표시되지 않습니다
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// 상세 헤더 열을 표시합니다
view.DisplayDetailsHeaderColumn = true;

// 모든 할당 행에 상세 헤더를 반복합니다
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### 또 보기

* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


