---
title: "PageSettings.FirstPageNumber"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PageSettings 속성. 인쇄할 첫 페이지 번호를 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.visualization/pagesettings/firstpagenumber/
---
## PageSettings.FirstPageNumber property

인쇄할 첫 페이지 번호를 가져오거나 설정합니다.

```csharp
public short FirstPageNumber { get; set; }
```

## 예제

&lt;see cref=\"Aspose.Tasks.Visualization.PageSettings\" /&gt;와 작업하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 설정을 가져옵니다
var settings = project.DefaultView.PageInfo.PageSettings;
// 몇몇 속성을 조정해 봅시다
// 페이지 방향이 세로인지 여부를 나타내는 값을 설정합니다; 페이지 방향이 가로이면 false를 반환합니다.
settings.IsPortrait = true;
// 인쇄할 너비 방향 페이지 수를 설정합니다.
settings.PagesInWidth = 5;
// 인쇄할 높이 방향 페이지 수를 설정합니다.
settings.PagesInHeight = 7;
// 인쇄를 조정할 정상 크기의 백분율을 설정합니다.
settings.PercentOfNormalSize = 200;
// 용지 크기를 설정합니다. <see cref=\"T:Aspose.Tasks.Visualization.PrinterPaperSize\" /> 열거형의 값 중 하나일 수 있습니다.
settings.PaperSize = PrinterPaperSize.PaperB4;
// 인쇄할 첫 페이지 번호를 설정합니다.
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

### 또 보기

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


