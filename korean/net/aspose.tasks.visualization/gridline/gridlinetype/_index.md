---
title: "Gridline.GridlineType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Gridline 속성. 그리드선의 유형인 GridlineType을 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.visualization/gridline/gridlinetype/
---
## Gridline.GridlineType property

그리드선의 유형 (`GridlineType`)을 가져오거나 설정합니다.

```csharp
public GridlineType GridlineType { get; set; }
```

## 예제

시각적 형식으로 저장하는 동안 그리드 라인을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // 그리드 라인의 유형을 설정합니다 (<see cref=\"P:Aspose.Tasks.Visualization.Gridline.GridlineType\" />).
    GridlineType = GridlineType.GanttRow, 
    // 그리드 라인의 <see cref=\"T:Aspose.Tasks.Visualization.LinePattern\" />을 설정합니다
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### 또 보기

* enum [GridlineType](../../gridlinetype/)
* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


