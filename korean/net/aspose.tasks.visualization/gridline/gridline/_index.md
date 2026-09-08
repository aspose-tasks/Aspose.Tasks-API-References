---
title: "Gridline.Gridline"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Gridline 생성자. Gridline 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.visualization/gridline/gridline/
---
## Gridline constructor

[`Gridline`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public Gridline()
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

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


