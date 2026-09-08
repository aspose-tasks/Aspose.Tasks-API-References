---
title: "열거형 GanttBarFillPattern"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.GanttBarFillPattern 열거형. 도형 채우기 패턴"
type: docs
weight: 3040
url: /ko/net/aspose.tasks.visualization/ganttbarfillpattern/
---
## GanttBarFillPattern enumeration

모양의 채우기 패턴입니다.

```csharp
public enum GanttBarFillPattern
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Hollow | `0` | 속이 빈 패턴. |
| SolidFill | `1` | 단색 채우기 패턴. |
| LightFill | `2` | 밝은 채우기 패턴. |
| MediumFill | `3` | 중간 채우기 패턴. |
| DarkFill | `4` | 어두운 채우기 패턴. |
| DiagonalLeft | `5` | 대각선 왼쪽 패턴 (왼쪽 위에서 오른쪽 아래로). |
| DiagonalRight | `6` | 대각선 오른쪽 패턴 (오른쪽 위에서 왼쪽 아래로). |
| DiagonalCross | `7` | 대각선 교차 패턴. |
| LineVertical | `8` | 수직 선 패턴. |
| LineHorizontal | `9` | 수평 선 패턴. |
| LineCross | `10` | 교차 선 패턴. |
| SolidFillWithDashedBorder | `11` | 실선과 점선 테두리 패턴. |

## 예제

Gantt 차트 프로젝트 보기의 사용자 정의 막대 스타일을 설정하는 방법을 보여줍니다.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // 프로젝트 보기의 사용자 정의 막대 컬렉션에 사용자 정의 막대 스타일을 추가합니다.
        view.CustomBarStyles.Add(custom);

        SimpleSaveOptions options = new MPPSaveOptions
        {
            WriteViewData = true
        };

        project.Save(OutDir + "ImplementCustomBarStyleWriting_out.mpp", options);
    }
    catch (NotSupportedException ex)
    {
        Console.WriteLine(
            ex.Message
            + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
    }
}

public static GanttBarStyle GetCustomBarStyle()
{
    var style = new GanttBarStyle
    {
        ShowForTaskUid = 1,
        MiddleShape = GanttBarMiddleShape.RectangleBottom,
        MiddleFillPattern = GanttBarFillPattern.MediumFill,
        MiddleShapeColor = Color.Blue,

        StartShape = GanttBarEndShape.ArrowDown,
        StartShapeColor = Color.Red,

        EndShape = GanttBarEndShape.ArrowUp,
        EndShapeColor = Color.Yellow,

        LeftField = Field.TaskResourceNames,
        RightField = Field.TaskName,
        TopField = Field.TaskStart,
        BottomField = Field.TaskFinish,
        InsideField = Field.TaskDuration
    };

    return style;
}
```

### 또 보기

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


