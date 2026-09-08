---
title: "GanttBarStyle.LeftBarTextConverter"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GanttBarStyle 속성. 작업 막대 왼쪽에 표시할 텍스트를 가져오기 위한 사용자 정의 변환기를 가져오거나 설정합니다. LeftField 속성의 값을 재정의합니다. MPP 형식에 저장되지 않습니다."
type: docs
weight: 100
url: /ko/net/aspose.tasks.visualization/ganttbarstyle/leftbartextconverter/
---
## GanttBarStyle.LeftBarTextConverter property

작업 막대 왼쪽에 표시할 텍스트를 가져오기 위한 사용자 정의 변환기를 가져오거나 설정합니다. [`LeftField`](../leftfield/) 속성의 값을 재정의합니다. MPP 형식에 저장되지 않습니다.

```csharp
public TaskBarTextConverter LeftBarTextConverter { get; set; }
```

## 예제

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

* delegate [TaskBarTextConverter](../../taskbartextconverter/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


