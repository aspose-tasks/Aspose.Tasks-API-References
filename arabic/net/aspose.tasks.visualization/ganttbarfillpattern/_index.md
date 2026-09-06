---
title: "تعداد GanttBarFillPattern"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Visualization.GanttBarFillPattern. نمط تعبئة الأشكال"
type: docs
weight: 3040
url: /ar/net/aspose.tasks.visualization/ganttbarfillpattern/
---
## GanttBarFillPattern enumeration

نمط تعبئة الشكل.

```csharp
public enum GanttBarFillPattern
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Hollow | `0` | نمط مجوف. |
| SolidFill | `1` | نمط تعبئة صلب. |
| LightFill | `2` | نمط تعبئة خفيف. |
| MediumFill | `3` | نمط تعبئة متوسط. |
| DarkFill | `4` | نمط تعبئة داكن. |
| DiagonalLeft | `5` | نمط قطري أيسر (من الأعلى الأيسر إلى الأسفل الأيمن). |
| DiagonalRight | `6` | نمط قطري أيمن (من الأعلى الأيمن إلى الأسفل الأيسر). |
| DiagonalCross | `7` | نمط تقاطع قطري. |
| LineVertical | `8` | نمط خط عمودي. |
| LineHorizontal | `9` | نمط خط أفقي. |
| LineCross | `10` | نمط تقاطع خطوط. |
| SolidFillWithDashedBorder | `11` | نمط صلب مع حد متقطع. |

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

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


