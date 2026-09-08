---
title: "클래스 PageLegend"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.PageLegend 클래스. 프로젝트 인쇄에 사용되는 페이지 레전드를 나타냅니다."
type: docs
weight: 3210
url: /ko/net/aspose.tasks.visualization/pagelegend/
---
## PageLegend class

프로젝트 인쇄에 사용되는 페이지 범례를 나타냅니다.

```csharp
public class PageLegend : HeaderFooterInfo
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [PageLegend](pagelegend/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | 부모 요소에 표시될 중앙 이미지를 가져오거나 설정합니다. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | 중앙 이미지의 표시 크기를 가져오거나 설정합니다. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | 부모 요소에 표시될 중앙 텍스트를 가져오거나 설정합니다. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | 부모 요소에 표시될 왼쪽 정렬된 이미지를 가져오거나 설정합니다. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | 왼쪽 이미지의 표시 크기를 가져오거나 설정합니다. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | 부모 요소에 표시될 왼쪽 정렬된 텍스트를 가져오거나 설정합니다. |
| [LegendOn](../../aspose.tasks.visualization/pagelegend/legendon/) { get; set; } | 레전드가 표시되는 페이지를 가져오거나 설정합니다. [`Legend`](../legend/) 열거형의 값 중 하나일 수 있습니다. |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | 부모 요소에 표시될 오른쪽 정렬된 이미지를 가져오거나 설정합니다. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | 오른쪽 이미지의 표시 크기를 가져오거나 설정합니다. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | 부모 요소에 표시될 오른쪽 정렬된 텍스트를 가져오거나 설정합니다. |
| [Width](../../aspose.tasks.visualization/pagelegend/width/) { get; set; } | 레전드의 왼쪽 부분(기본적으로 프로젝트 이름과 날짜를 포함)의 너비를 센티미터 단위로 가져오거나 설정합니다. |

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

### 또 보기

* class [HeaderFooterInfo](../headerfooterinfo/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


