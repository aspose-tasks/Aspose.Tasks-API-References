---
title: "클래스 Gridline"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.Gridline 클래스. 프로젝트 보기에서 나타나는 수평 또는 수직 선"
type: docs
weight: 3100
url: /ko/net/aspose.tasks.visualization/gridline/
---
## Gridline class

프로젝트 보기에서 나타나는 가로 또는 세로 선입니다.

```csharp
public class Gridline
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Gridline](gridline/)() | `Gridline` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Color](../../aspose.tasks.visualization/gridline/color/) { get; set; } | 그리드라인의 [`Color`](./color/)을 가져오거나 설정합니다. |
| [GridlineType](../../aspose.tasks.visualization/gridline/gridlinetype/) { get; set; } | 그리드라인의 유형([`GridlineType`](./gridlinetype/))을 가져오거나 설정합니다. |
| [Pattern](../../aspose.tasks.visualization/gridline/pattern/) { get; set; } | 그리드라인의 [`LinePattern`](../linepattern/)을 가져오거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| override [Equals](../../aspose.tasks.visualization/gridline/equals/)(object) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 플래그를 반환합니다. |
| override [GetHashCode](../../aspose.tasks.visualization/gridline/gethashcode/)() | `Gridline` 클래스 인스턴스에 대한 해시 코드 값을 반환합니다. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


