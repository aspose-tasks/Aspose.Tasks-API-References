---
title: "GanttBarStyle.ParentStyle"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GanttBarStyle 속성. 사용자 지정 작업별 스타일에 대한 상위 또는 공통 스타일을 가져오거나 설정합니다."
type: docs
weight: 160
url: /ko/net/aspose.tasks.visualization/ganttbarstyle/parentstyle/
---
## GanttBarStyle.ParentStyle property

사용자 지정 작업별 스타일에 대한 상위(또는 공통) 스타일을 가져오거나 설정합니다.

```csharp
public GanttBarStyle ParentStyle { get; set; }
```

## 비고

작업은 서로 다른 상위 스타일을 가진 여러 사용자 지정 스타일을 가질 수 있습니다. 예를 들어, "Critical" 상위 스타일을 가진 사용자 지정 스타일과 "Normal" 상위 스타일을 가진 다른 스타일을 가진 작업을 고려해 보세요. 간단히 말해, 작업이 중요하면 첫 번째 스타일이 적용됩니다. 작업이 비중요 상태가 되면 두 번째 스타일이 적용됩니다(이 논리는 Microsoft Project Professional에서 상속됩니다).

## 예제

뷰의 사용자 정의 막대 스타일을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CustomBarStyle.mpp");

var view = (GanttChartView)project.DefaultView;
Console.WriteLine("Custom bar styles count: {0}", view.CustomBarStyles.Count);

var style1 = view.CustomBarStyles[0];
Console.WriteLine("Style1.ParentStyle Name: {0}", style1.ParentStyle.Name);
Console.WriteLine("Style1.LeftField: {0}", style1.LeftField);
Console.WriteLine("Style1.RightField: {0}", style1.RightField);
Console.WriteLine("Style1.TopField: {0}", style1.TopField);
Console.WriteLine("Style1.BottomField: {0}", style1.BottomField);
Console.WriteLine("Style1.InsideField: {0}", style1.InsideField);
Console.WriteLine("Style1.From: {0}", style1.From);
Console.WriteLine("Style1.To: {0}", style1.To);
Console.WriteLine("Style1.Row: {0}", style1.Row);

var style2 = view.CustomBarStyles[1];
Console.WriteLine("Style2.LeftField: {0}", style2.LeftField);
Console.WriteLine("Style2.RightField: {0}", style2.RightField);
Console.WriteLine("Style2.TopField: {0}", style2.TopField);
Console.WriteLine("Style2.BottomField: {0}", style2.BottomField);
Console.WriteLine("Style2.InsideField: {0}", style2.InsideField);
Console.WriteLine("Style2.From: {0}", style2.From);
Console.WriteLine("Style2.To: {0}", style2.To);
Console.WriteLine("Style2.Row: {0}", style1.Row);

var style3 = view.CustomBarStyles[2];
Console.WriteLine("Style3.LeftField: {0}", style3.LeftField);
Console.WriteLine("Style3.RightField: {0}", style3.RightField);
Console.WriteLine("Style3.TopField: {0}", style3.TopField);
Console.WriteLine("Style3.BottomField: {0}", style3.BottomField);
Console.WriteLine("Style3.InsideField: {0}", style3.InsideField);

Console.WriteLine("Style3.StartShape: {0}", style3.StartShape);
Console.WriteLine("Style3.StartShapeType: {0}", style3.StartShapeType);
Console.WriteLine("Style3.StartShapeColor: {0}", style3.StartShapeColor);

Console.WriteLine("Style3.EndShape: {0}", style3.EndShape);
Console.WriteLine("Style3.EndShapeType: {0}", style3.EndShapeType);
Console.WriteLine("Style3.EndShapeColor: {0}", style3.EndShapeColor);

Console.WriteLine("Style3.MiddleShape: {0}", style3.MiddleShape);
Console.WriteLine("Style3.MiddleFillPattern: {0}", style3.MiddleFillPattern);
Console.WriteLine("Style3.MiddleShapeColor: {0}", style3.MiddleShapeColor);
Console.WriteLine("Style3.From: {0}", style3.From);
Console.WriteLine("Style3.To: {0}", style3.To);
Console.WriteLine("Style3.Row: {0}", style1.Row);
```

### 또 보기

* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


