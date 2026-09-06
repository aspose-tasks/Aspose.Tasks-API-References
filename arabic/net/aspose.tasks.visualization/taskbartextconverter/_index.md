---
title: "المندوب TaskBarTextConverter"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "محول مخصص لبيانات المهام إلى نص الشريط"
type: docs
weight: 3380
url: /ar/net/aspose.tasks.visualization/taskbartextconverter/
---
## TaskBarTextConverter delegate

محول مخصص لبيانات المهمة إلى نص الشريط.

```csharp
public delegate string TaskBarTextConverter(Task task);
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| مهمة | مهمة | المهمة التي سيتم عرض نص شريطها. |

### قيمة الإرجاع

النص الذي سيتم عرضه لشريط يتوافق مع المهمة المحددة.

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

* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


