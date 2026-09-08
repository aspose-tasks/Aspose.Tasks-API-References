---
title: "PageInfo.Legend"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PageInfo 속성. 페이지 범례의 렌더링 옵션을 지정하는 PageLegend 클래스의 인스턴스를 가져오거나 설정합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks.visualization/pageinfo/legend/
---
## PageInfo.Legend property

페이지 범례의 렌더링 옵션을 지정하는 [`PageLegend`](../../pagelegend/) 클래스의 인스턴스를 가져옵니다.

```csharp
public PageLegend Legend { get; set; }
```

## 비고

현재는 Gantt 차트 보기에서만 적용됩니다.

## 예제

페이지 레전드 정보를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// 페이지 레전드 정보를 읽습니다.
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// 레전드 수정도 지원됩니다.
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

MS Project 뷰의 페이지 정보를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 기본 보기를 수정합니다.
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// 여백을 수정합니다.
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// 페이지 설정을 수정합니다.
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// 페이지 뷰 설정을 수정합니다.
// 노트를 인쇄할지 여부를 나타내는 값을 설정합니다.
info.PageViewSettings.PrintNotes = true;

var header = new HeaderFooterInfo
{
    LeftText = "Left header text",
    CenteredText = "Centered header text",
    RightText = "Right header text"
};
var legend = new PageLegend
{
    LeftText =  "Left legend text",
    CenteredText = "Centered legend text",
    RightText = "Right legend text"
};
var footer = new HeaderFooterInfo
{
    LeftText = "Left footer text",
    CenteredText = "Centered footer text",
    RightText = "Right footer text"
};

info.Header = header;
info.Legend = legend;
info.Footer = footer;

// 프로젝트 작업...
```

### 또 보기

* class [PageLegend](../../pagelegend/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


