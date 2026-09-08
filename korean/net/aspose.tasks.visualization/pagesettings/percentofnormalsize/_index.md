---
title: "PageSettings.PercentOfNormalSize"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PageSettings 속성. 인쇄를 조정하기 위한 정상 크기의 백분율을 가져오거나 설정합니다."
type: docs
weight: 90
url: /ko/net/aspose.tasks.visualization/pagesettings/percentofnormalsize/
---
## PageSettings.PercentOfNormalSize property

인쇄를 조정할 정상 크기의 백분율을 가져오거나 설정합니다.

```csharp
public int PercentOfNormalSize { get; set; }
```

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


