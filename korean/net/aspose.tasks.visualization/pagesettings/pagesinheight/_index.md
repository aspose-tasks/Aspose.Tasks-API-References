---
title: "PageSettings.PagesInHeight"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PageSettings 속성. 인쇄할 높이 페이지 수를 가져오거나 설정합니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks.visualization/pagesettings/pagesinheight/
---
## PageSettings.PagesInHeight property

인쇄할 높이 방향 페이지 수를 가져오거나 설정합니다.

```csharp
public int PagesInHeight { get; set; }
```

## 예제

'Fit X to Y pages' 옵션을 사용하여 뷰를 렌더링하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.TaskUsage);

view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = false;
// 뷰가 높이 기준으로 2페이지 이하로 렌더링되도록 지정합니다.
view.PageInfo.PageSettings.PagesInHeight = 2;
// 뷰가 가로 기준으로 1페이지로 렌더링되도록 지정합니다.
view.PageInfo.PageSettings.PagesInWidth = 1;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView,
    StartDate =  new DateTime(2000, 04, 1),
    EndDate = new DateTime(2000, 12, 31)
};

project.Save(OutDir + "PrintViewWithFitToPages_out.pdf", saveOptions);
```

### 또 보기

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


