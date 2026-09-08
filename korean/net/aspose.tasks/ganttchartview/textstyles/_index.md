---
title: "GanttChartView.TextStyles"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GanttChartView 속성. Gantt 차트 뷰의 TextStyle 목록을 가져오거나 설정합니다."
type: docs
weight: 170
url: /ko/net/aspose.tasks/ganttchartview/textstyles/
---
## GanttChartView.TextStyles property

Gantt 차트 뷰의 [`TextStyle`](../../../aspose.tasks.visualization/textstyle/) 목록을 가져오거나 설정합니다.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## 예제

Gantt 차트 텍스트 스타일을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// Gantt 차트 뷰의 텍스트 스타일을 반복합니다.
foreach (var style in view.TextStyles)
{
    Console.WriteLine("Style Item Type: " + style.ItemType);
    Console.WriteLine("Style Font name: " + style.Font.FontFamily);
    Console.WriteLine();
}
```

### 또 보기

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


