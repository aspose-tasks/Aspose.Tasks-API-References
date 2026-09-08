---
title: "PageLegend.Width"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PageLegend 속성. 레전드의 기본값으로 프로젝트 이름과 날짜를 포함하는 왼쪽 부분의 너비를 센티미터 단위로 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.visualization/pagelegend/width/
---
## PageLegend.Width property

레전드의 왼쪽 부분(기본적으로 프로젝트 이름과 날짜를 포함)의 너비를 센티미터 단위로 가져오거나 설정합니다.

```csharp
public double Width { get; set; }
```

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentOutOfRangeException | 값을 0보다 작은 값으로 설정하려고 할 때. |

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

* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


