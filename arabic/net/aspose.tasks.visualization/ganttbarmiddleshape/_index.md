---
title: "تعداد GanttBarMiddleShape"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Visualization.GanttBarMiddleShape. يحدد الشكل الأوسط للعمود"
type: docs
weight: 3050
url: /ar/net/aspose.tasks.visualization/ganttbarmiddleshape/
---
## GanttBarMiddleShape enumeration

يحدد الشكل الأوسط للشريط.

```csharp
public enum GanttBarMiddleShape
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| LineBottom | `7` | يشير إلى شكل خط محاذى إلى الأسفل. |
| LineMiddle | `6` | يشير إلى شكل خط محاذى إلى الوسط. |
| LineTop | `5` | يشير إلى شكل خط محاذى إلى الأعلى. |
| None | `0` | يشير إلى شكل فارغ. |
| RectangleBar | `1` | يشير إلى شكل عمود مستطيل بارتفاع كامل. |
| RectangleBottom | `4` | يشير إلى شكل عمود مستطيل نصف الارتفاع محاذى إلى الأسفل. |
| RectangleMiddle | `3` | يشير إلى شكل عمود مستطيل بارتفاع ثلث محاذى إلى الوسط. |
| RectangleTop | `2` | يشير إلى شكل شريط مستطيل نصف الارتفاع محاذى إلى الأعلى. |

## الأمثلة

يوضح كيفية تعيين أنماط أشرطة مخصصة لعرض مشروع مخطط جانت.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // أضف نمط الشريط المخصص إلى مجموعة الأشرطة المخصصة لعرض المشروع
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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


