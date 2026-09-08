---
title: "PageSettings.AdjustToPercentOfNormalSize"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PageSettings 속성. 정상 크기의 지정된 백분율 PercentOfNormalSize에 인쇄를 조정할지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/
---
## PageSettings.AdjustToPercentOfNormalSize property

지정된 백분율 ([`PercentOfNormalSize`](../percentofnormalsize/))에 인쇄를 조정할지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool AdjustToPercentOfNormalSize { get; set; }
```

## 비고

프로젝트가 HTML 형식으로 렌더링될 때는 적용되지 않습니다.

## 예제

지정된 배율을 사용하여 뷰를 렌더링하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Input.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

// 지정된 배율을 사용하여 뷰를 확대/축소해야 함을 나타내는 값을 설정합니다.
view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = true;
// 배율을 지정합니다.
view.PageInfo.PageSettings.PercentOfNormalSize = 33;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "PrintViewWithSpecifiedScaleFactor_out.pdf", saveOptions);
```

### 또 보기

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


