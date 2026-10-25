---
title: "PageLegend.LegendOn"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PageLegend 속성. 범례가 표시되는 페이지를 가져오거나 설정합니다. Legend 열거형의 값 중 하나일 수 있습니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.visualization/pagelegend/legendon/
---
## PageLegend.LegendOn property

범례가 표시되는 페이지를 가져오거나 설정합니다. [`Legend`](../../legend/) 열거형의 값 중 하나일 수 있습니다.

```csharp
public Legend LegendOn { get; set; }
```

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

* enum [Legend](../../legend/)
* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


