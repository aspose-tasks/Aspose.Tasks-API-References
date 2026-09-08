---
title: "열거형 PrinterPaperSize"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.PrinterPaperSize 열거형. 인쇄에 사용되는 용지 크기를 지정합니다."
type: docs
weight: 3280
url: /ko/net/aspose.tasks.visualization/printerpapersize/
---
## PrinterPaperSize enumeration

인쇄에 사용되는 용지 크기를 지정합니다.

```csharp
public enum PrinterPaperSize
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Custom | `1` | 용지 크기가 사용자가 정의했음을 나타냅니다. |
| PaperLetter | `1` | Envelope Letter 프린터 용지 크기를 표시합니다 (8.5 in. by 11 in.). |
| PaperLetterSmall | `2` | Small Letter 프린터 용지 크기를 표시합니다 (8.5 in. by 11 in.). |
| PaperTabloid | `3` | Tabloid 프린터 용지 크기를 표시합니다 (11 in. by 17 in.). |
| PaperLedger | `4` | Ledger 프린터 용지 크기를 표시합니다 (17 in. by 11 in.). |
| PaperLegal | `5` | Envelope legal 프린터 용지 크기를 표시합니다 (8.5 in. by 14 in.). |
| PaperStatement | `6` | Statement 프린터 용지 크기를 표시합니다 (5.5 in. by 8.5 in.). |
| PaperExecutive | `7` | Envelope executive 프린터 용지 크기를 표시합니다 (7.25 in. by 10.5 in.). |
| PaperA3 | `8` | A3 프린터 용지 크기를 표시합니다 (297 mm by 420 mm). |
| PaperA4 | `9` | A4 프린터 용지 크기를 표시합니다 (210 mm by 297 mm). |
| PaperA4Small | `10` | Small A4 프린터 용지 크기를 표시합니다 (210 mm by 297 mm). |
| PaperA5 | `11` | A5 프린터 용지 크기를 표시합니다 (148 mm by 210 mm). |
| PaperB4 | `12` | B4 프린터 용지 크기를 표시합니다 (250 mm by 353 mm). |
| PaperB5 | `13` | B5 프린터 용지 크기를 표시합니다 (176 mm by 250 mm). |
| PaperFolio | `14` | Folio 프린터 용지 크기를 표시합니다 (8.5 in. by 13 in.). |
| PaperQuarto | `15` | Quarto 프린터 용지 크기를 표시합니다 (215 mm by 275 mm). |
| PaperStandard10x14 | `16` | Standard 프린터 용지 크기를 표시합니다 (10 in. by 14 in.). |
| PaperStandard11x17 | `17` | Standard 프린터 용지 크기를 표시합니다 (11 in. by 17 in.). |
| PaperNote | `18` | Note 프린터 용지 크기를 표시합니다 (8.5 in. by 11 in.). |
| PaperEnvelope10 | `20` | Envelope10 프린터 용지 크기를 표시합니다 (4.125 in. by 9.5 in.). |
| PaperCSheet | `24` | C paper 프린터 용지 크기를 표시합니다 (17 in. by 22 in.). |
| PaperDSheet | `25` | D paper 프린터 용지 크기를 표시합니다 (22 in. by 34 in.). |
| PaperESheet | `26` | E paper 프린터 용지 크기를 표시합니다 (34 in. by 44 in.). |
| PaperEnvelopeMonarch | `37` | Envelope Monarch 프린터 용지 크기를 표시합니다 (3.875 in. by 7.5 in.). |
| PaperStandard9x11 | `44` | Standard 프린터 용지 크기를 표시합니다 (9 in. by 11 in.). |
| PaperStandard10x11 | `45` | Standard 프린터 용지 크기를 표시합니다 (10 in. by 11 in.). |
| PaperStandard15x11 | `46` | 표준 프린터 용지 크기(15인치 × 11인치)를 나타냅니다. |
| PaperA2 | `66` | A2 프린터 용지 크기(420 mm × 594 mm)를 나타냅니다. |

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


