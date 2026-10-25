---
title: "تعداد GanttBarEndShape"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.Visualization.GanttBarEndShape enum. يمثل الشكل النهائي في الأشرطة ونقاط التقدم في خطوط التقدم."
type: docs
weight: 3030
url: /ar/net/aspose.tasks.visualization/ganttbarendshape/
---
## GanttBarEndShape enumeration

يمثل الشكل النهائي في الأشرطة ونقاط التقدم في خطوط التقدم.

```csharp
public enum GanttBarEndShape
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| ArrowDown | `14` | يشير إلى سهم يشير إلى الأسفل شكل نهاية شريط Gantt. |
| ArrowUp | `8` | يشير إلى سهم يشير إلى الأعلى شكل نهاية شريط Gantt. |
| CaretDownTop | `9` | يشير إلى إشارة تشير إلى الأسفل على النصف العلوي من الشريط شكل نهاية شريط Gantt. |
| CaretUpBottom | `10` | يشير إلى إشارة تشير إلى الأعلى على النصف السفلي من الشريط شكل نهاية شريط Gantt. |
| Circle | `19` | يشير إلى دائرة شكل نهاية شريط Gantt. |
| CircleArrowDown | `18` | يشير إلى سهم محاط بدائرة يشير إلى الأسفل شكل نهاية شريط Gantt. |
| CircleArrowUp | `17` | يشير إلى سهم محاط بدائرة يشير إلى الأعلى شكل نهاية شريط Gantt. |
| CircleDiamond | `13` | يشير إلى ماسة محاطة بدائرة شكل نهاية شريط Gantt. |
| CircleTriangleDown | `16` | يشير إلى مثلث محاط بدائرة يشير إلى الأسفل شكل نهاية شريط Gantt. |
| CircleTriangleUp | `15` | يشير إلى مثلث محاط بدائرة يشير إلى الأعلى شكل نهاية شريط Gantt. |
| Diamond | `3` | يشير إلى ماسة شكل نهاية شريط Gantt. |
| HouseDown | `2` | يشير إلى منزل مقلوب شكل نهاية شريط Gantt. |
| HouseUp | `1` | يشير إلى منزل شكل نهاية شريط Gantt. |
| LeftBracket | `21` | يشير إلى قوس أيسر شكل نهاية شريط Gantt. |
| LeftFade | `23` | يشير إلى تلاشي أيسر شكل نهاية شريط Gantt. |
| LineShape | `11` | يشير إلى خط شكل نهاية شريط Gantt. |
| NoBarEndShape | `0` | يشير إلى لا شيء شكل نهاية شريط Gantt. |
| RightBracket | `22` | يشير إلى قوس أيمن شكل نهاية شريط Gantt. |
| RightFade | `24` | يشير إلى تلاشي أيمن شكل نهاية شريط Gantt. |
| Square | `12` | يشير إلى مربع شكل نهاية شريط Gantt. |
| Star | `20` | يشير إلى نجمة شكل نهاية شريط Gantt. |
| TriangleDown | `5` | يشير إلى مثلث يشير إلى الأسفل شكل نهاية شريط Gantt. |
| TriangleLeft | `7` | يشير إلى شكل مثلث يتجه إلى اليسار في نهاية شريط مخطط جانت. |
| TriangleRight | `6` | يشير إلى شكل مثلث يتجه إلى اليمين في نهاية شريط مخطط جانت. |
| TriangleUp | `4` | يشير إلى مثلث محاط بدائرة يشير إلى الأعلى شكل نهاية شريط Gantt. |

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


