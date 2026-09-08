---
title: "델리게이트 TaskBarTextConverter"
second_title: "Aspose.Tasks for .NET API 참조"
description: "작업 데이터에서 막대 텍스트로 변환하는 사용자 지정 변환기"
type: docs
weight: 3380
url: /ko/net/aspose.tasks.visualization/taskbartextconverter/
---
## TaskBarTextConverter delegate

작업 데이터를 막대 텍스트로 변환하는 사용자 지정 변환기입니다.

```csharp
public delegate string TaskBarTextConverter(Task task);
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 작업 | 작업 | 작업 막대 텍스트가 렌더링될 작업. |

### 반환 값

지정된 작업에 해당하는 막대에 렌더링할 텍스트.

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

* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


