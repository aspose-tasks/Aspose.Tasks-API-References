---
title: "열거형 GanttBarEndShape"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.GanttBarEndShape 열거형. 막대와 진행 라인에서 진행 지점의 끝 모양을 나타냅니다."
type: docs
weight: 3030
url: /ko/net/aspose.tasks.visualization/ganttbarendshape/
---
## GanttBarEndShape enumeration

막대와 진행선의 진행 지점에서 끝 모양을 나타냅니다.

```csharp
public enum GanttBarEndShape
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| ArrowDown | `14` | 아래쪽을 가리키는 화살표 Gantt bar end shape를 표시합니다. |
| ArrowUp | `8` | 위쪽을 가리키는 화살표 Gantt bar end shape를 표시합니다. |
| CaretDownTop | `9` | 막대 상단 절반에 아래쪽을 가리키는 캐럿 Gantt bar end shape를 표시합니다. |
| CaretUpBottom | `10` | 막대 하단 절반에 위쪽을 가리키는 캐럿 Gantt bar end shape를 표시합니다. |
| Circle | `19` | 원형 Gantt bar end shape를 표시합니다. |
| CircleArrowDown | `18` | 아래쪽을 가리키는 원형 화살표 Gantt bar end shape를 표시합니다. |
| CircleArrowUp | `17` | 위쪽을 가리키는 원형 화살표 Gantt bar end shape를 표시합니다. |
| CircleDiamond | `13` | 원형 다이아몬드 Gantt bar end shape를 표시합니다. |
| CircleTriangleDown | `16` | 아래쪽을 가리키는 원형 삼각형 Gantt bar end shape를 표시합니다. |
| CircleTriangleUp | `15` | 위쪽을 가리키는 원형 삼각형 Gantt bar end shape를 표시합니다. |
| Diamond | `3` | 다이아몬드 Gantt bar end shape를 표시합니다. |
| HouseDown | `2` | 거꾸로 된 집 모양 Gantt bar end shape를 표시합니다. |
| HouseUp | `1` | 집 모양 Gantt bar end shape를 표시합니다. |
| LeftBracket | `21` | 왼쪽 괄호 Gantt bar end shape를 표시합니다. |
| LeftFade | `23` | 왼쪽 페이드 Gantt bar end shape를 표시합니다. |
| LineShape | `11` | 선형 Gantt bar end shape를 표시합니다. |
| NoBarEndShape | `0` | 없음 Gantt bar end shape를 표시합니다. |
| RightBracket | `22` | 오른쪽 괄호 Gantt bar end shape를 표시합니다. |
| RightFade | `24` | 오른쪽 페이드 Gantt bar end shape를 표시합니다. |
| Square | `12` | 정사각형 Gantt bar end shape를 표시합니다. |
| Star | `20` | 별 모양 Gantt bar end shape를 표시합니다. |
| TriangleDown | `5` | 아래쪽을 가리키는 삼각형 Gantt bar end shape를 표시합니다. |
| TriangleLeft | `7` | 왼쪽을 가리키는 삼각형 Gantt 막대 끝 모양을 나타냅니다. |
| TriangleRight | `6` | 오른쪽을 가리키는 삼각형 Gantt 막대 끝 모양을 나타냅니다. |
| TriangleUp | `4` | 위쪽을 가리키는 원형 삼각형 Gantt bar end shape를 표시합니다. |

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


