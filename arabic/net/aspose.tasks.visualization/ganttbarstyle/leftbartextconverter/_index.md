---
title: "GanttBarStyle.LeftBarTextConverter"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية GanttBarStyle. يحصل أو يضبط محولًا معرفًا من قبل المستخدم للحصول على النص لعرضه على يسار شريط المهام. يتجاوز قيمة خاصية LeftField. لا يتم حفظه في تنسيق MPP"
type: docs
weight: 100
url: /ar/net/aspose.tasks.visualization/ganttbarstyle/leftbartextconverter/
---
## GanttBarStyle.LeftBarTextConverter property

يحصل أو يضبط محولًا معرفًا من قبل المستخدم للحصول على النص لعرضه على يسار شريط المهمة. يتجاوز قيمة خاصية [`LeftField`](../leftfield/). لا يتم حفظه في تنسيق MPP.

```csharp
public TaskBarTextConverter LeftBarTextConverter { get; set; }
```

## الأمثلة

يوضح كيفية استخدام أنماط الأشرطة المخصصة لعرض مخطط جانت.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var ganttChartView = (GanttChartView)project.Views.First(v => v.Name == "Gantt &Chart");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.ViewSettings = ganttChartView;

// يمكن أن تكون أنماط الأشرطة إما خاصة بالمهمة (تقع في GanttChartView.CustomBarStyles)
// من النوع الخاص بالفئة (تقع في GanttChartView.BarStyles)
foreach (GanttBarStyle ganttBarStyle in ganttChartView.CustomBarStyles)
{
    if (ganttBarStyle.ShowForTaskUid != 4)
    {
        continue;
    }

    // لأغراض العرض نقوم بتعديل النمط للمهمة ذات المعرف الفريد = 4
    // هنا نحدد الحقل (TaskName) ليتم عرضه إلى يسار شريط المهمة.
    ganttBarStyle.LeftField = Field.TaskName;
    // هنا نحدد محولًا مخصصًا للتحكم في النص الذي يجب عرضه داخل شريط المهمة.
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

    // لأغراض العرض نقوم بتعديل الأنماط المطبقة على مهام المعالم.

    ganttBarStyle.StartShape = GanttBarEndShape.Diamond;
    ganttBarStyle.RightField = Field.TaskActualFinish;
    ganttBarStyle.TopBarTextConverter = task => task.Get(Tsk.ActualStart).Day.ToString();
}

project.Save(OutDir + "WorkWithGanttChartViewBarStyles_out.pdf", saveOptions);
```

### انظر أيضًا

* delegate [TaskBarTextConverter](../../taskbartextconverter/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


