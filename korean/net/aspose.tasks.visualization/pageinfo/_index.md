---
title: "클래스 PageInfo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.PageInfo 클래스. MPP 파일 형식에 존재하고 인쇄에 사용되는 페이지 설정 데이터를 나타냅니다."
type: docs
weight: 3200
url: /ko/net/aspose.tasks.visualization/pageinfo/
---
## PageInfo class

인쇄에 사용되는 MPP 파일 형식에 존재하는 페이지 설정 데이터를 나타냅니다.

```csharp
public class PageInfo
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PageInfo](pageinfo/)() | `PageInfo` 클래스의 새 인스턴스를 초기화합니다. MPP 파일 형식에 존재하고 인쇄에 사용되는 페이지 설정 데이터를 나타냅니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Footer](../../aspose.tasks.visualization/pageinfo/footer/) { get; set; } | 푸터 데이터를 나타내는 [`HeaderFooterInfo`](../headerfooterinfo/) 클래스의 인스턴스를 가져오거나 설정합니다. |
| [Header](../../aspose.tasks.visualization/pageinfo/header/) { get; set; } | 헤더 데이터를 나타내는 [`HeaderFooterInfo`](../headerfooterinfo/) 클래스의 인스턴스를 가져오거나 설정합니다. |
| [Legend](../../aspose.tasks.visualization/pageinfo/legend/) { get; set; } | 페이지 레전드의 렌더링 옵션을 지정하는 [`PageLegend`](../pagelegend/) 클래스의 인스턴스를 가져오거나 설정합니다. |
| [Margins](../../aspose.tasks.visualization/pageinfo/margins/) { get; } | 페이지 여백을 지정하는 [`PageMargins`](../pagemargins/) 클래스의 인스턴스를 가져옵니다. |
| [Name](../../aspose.tasks.visualization/pageinfo/name/) { get; } | 설정 데이터가 사용되는 뷰의 이름을 가져옵니다. |
| [PageSettings](../../aspose.tasks.visualization/pageinfo/pagesettings/) { get; } | 페이지 인쇄 설정을 지정하는 [`PageSettings`](./pagesettings/) 클래스의 인스턴스를 가져옵니다. |
| [PageViewSettings](../../aspose.tasks.visualization/pageinfo/pageviewsettings/) { get; } | 페이지 뷰 인쇄 설정을 지정하는 [`PageViewSettings`](./pageviewsettings/) 클래스의 인스턴스를 가져옵니다. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


