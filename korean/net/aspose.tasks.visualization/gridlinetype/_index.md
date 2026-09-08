---
title: "열거형 GridlineType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.GridlineType 열거형. 그리드라인 유형"
type: docs
weight: 3110
url: /ko/net/aspose.tasks.visualization/gridlinetype/
---
## GridlineType enumeration

그리드선 유형입니다.

```csharp
public enum GridlineType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| GanttRow | `0` | Gantt 행 그리드 라인 유형의 그리드라인을 나타냅니다. |
| TopTierColumn | `1` | 상위 계층 열 그리드 라인 유형의 그리드라인을 나타냅니다. |
| BottomTierColumn | `2` | 하위 계층 열 그리드 라인 유형의 그리드라인을 나타냅니다. |
| SheetRow | `3` | 시트 행 그리드 라인 유형의 그리드라인을 나타냅니다. |
| SheetColumn | `4` | 시트 열 그리드 라인 유형의 그리드라인을 나타냅니다. |
| UsageRow | `5` | 사용 행 그리드 라인 유형의 그리드라인을 나타냅니다. |
| UsageColumn | `6` | 사용 열 그리드 라인 유형의 그리드라인을 나타냅니다. |
| GanttTitleVertical | `7` | Gantt 제목 수직 그리드 라인 유형을 나타냅니다. |
| GanttTitleHorizontal | `8` | Gantt 제목 수평 그리드 라인 유형을 나타냅니다. |
| BarRows | `9` | 막대 행 그리드 라인 유형을 나타냅니다. |
| GanttProjectStart | `10` | Gantt 프로젝트 시작 그리드 라인 유형을 나타냅니다. |
| GanttProjectFinish | `11` | Gantt 프로젝트 종료 그리드 라인 유형을 나타냅니다. |
| GanttStatusDate | `12` | Gantt 상태 날짜 그리드 라인 유형을 나타냅니다. |
| GanttCurrentDate | `13` | Gantt 현재 날짜 그리드 라인 유형을 나타냅니다. |
| GanttPageBreaks | `14` | Gantt 페이지 구분 그리드 라인 유형을 나타냅니다. |
| MiddleTierColumn | `15` | 중간 계층 열 그리드 라인 유형을 나타냅니다. |

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


