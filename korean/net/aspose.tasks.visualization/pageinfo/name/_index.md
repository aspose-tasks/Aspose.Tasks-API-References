---
title: "PageInfo.Name"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PageInfo 속성. 설정 데이터가 사용되는 보기의 이름을 가져옵니다."
type: docs
weight: 60
url: /ko/net/aspose.tasks.visualization/pageinfo/name/
---
## PageInfo.Name property

설정 데이터가 사용되는 뷰의 이름을 가져옵니다.

```csharp
public string Name { get; }
```

## 예제

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

* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


