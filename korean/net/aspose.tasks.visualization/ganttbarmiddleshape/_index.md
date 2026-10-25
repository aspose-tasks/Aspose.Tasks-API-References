---
title: "열거형 GanttBarMiddleShape"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.GanttBarMiddleShape 열거형. 막대의 중간 모양을 지정합니다."
type: docs
weight: 3050
url: /ko/net/aspose.tasks.visualization/ganttbarmiddleshape/
---
## GanttBarMiddleShape enumeration

막대의 중간 모양을 지정합니다.

```csharp
public enum GanttBarMiddleShape
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| LineBottom | `7` | 하단 정렬된 선 모양을 나타냅니다. |
| LineMiddle | `6` | 중앙 정렬된 선 모양을 나타냅니다. |
| LineTop | `5` | 상단 정렬된 선 모양을 나타냅니다. |
| None | `0` | 빈 모양을 나타냅니다. |
| RectangleBar | `1` | 전체 높이 사각형 막대 모양을 나타냅니다. |
| RectangleBottom | `4` | 아래쪽 정렬된 절반 높이 사각형 막대 모양을 나타냅니다. |
| RectangleMiddle | `3` | 중앙 정렬된 1/3 높이 사각형 막대 모양을 나타냅니다. |
| RectangleTop | `2` | 상단 정렬된 절반 높이 사각형 막대 모양을 나타냅니다. |

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

Gantt 차트 보기에서 사용자 정의 막대 스타일을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var ganttChartView = (GanttChartView)project.Views.First(v => v.Name == "Gantt &Chart");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.ViewSettings = ganttChartView;

// 막대 스타일은 작업별일 수 있으며 (GanttChartView.CustomBarStyles에 위치함)
// 카테고리별 (GanttChartView.BarStyles에 위치함)
foreach (GanttBarStyle ganttBarStyle in ganttChartView.CustomBarStyles)
{
    if (ganttBarStyle.ShowForTaskUid != 4)
    {
        continue;
    }

    // 시연을 위해 고유 ID = 4인 작업의 스타일을 수정하고 있습니다.
    // 여기서는 필드 (TaskName)를 작업 막대 왼쪽에 표시하도록 설정합니다.
    ganttBarStyle.LeftField = Field.TaskName;
    // 여기서는 사용자 정의 변환기를 설정하여 작업 막대 내부에 표시될 텍스트를 제어합니다.
    ganttBarStyle.InsideBarTextConverter = task => "Hours rem.: " + (int)task.Get(Tsk.RemainingWork).TimeSpan.TotalHours;

    ganttBarStyle.MiddleShapeColor = Color.Green;
    ganttBarStyle.MiddleShape = GanttBarMiddleShape.LineTop;
    ganttBarStyle.StartShape = GanttBarEndShape.LeftBracket;
    ganttBarStyle.StartShapeColor = Color.Aqua;
    ganttBarStyle.EndShape = GanttBarEndShape.RightBracket;
    ganttBarStyle.EndShapeColor = Color.Aquamarine;
}

foreach (GanttBarStyle ganttBarStyle in ganttChartView.BarStyles)
{
    if (!ganttBarStyle.ShowForCategories.Contains(GanttBarShowFor.Milestone))
    {
        continue;
    }

    // 시연을 위해 마일스톤 작업에 적용되는 스타일을 수정하고 있습니다.

    ganttBarStyle.StartShape = GanttBarEndShape.Diamond;
    ganttBarStyle.RightField = Field.TaskActualFinish;
    ganttBarStyle.TopBarTextConverter = task => task.Get(Tsk.ActualStart).Day.ToString();
}

project.Save(OutDir + "WorkWithGanttChartViewBarStyles_out.pdf", saveOptions);
```

### 또 보기

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


