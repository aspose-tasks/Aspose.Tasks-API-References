---
title: "تعداد Shape"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.Visualization.Shape enum. شكل علامة في بداية أو نهاية نمط الشريط ليتم عرضه عند حفظ بيانات العرض إلى بعض صيغ SaveFileFormat"
type: docs
weight: 3360
url: /ar/net/aspose.tasks.visualization/shape/
---
## Shape enumeration

شكل علامة في بداية أو نهاية نمط الشريط ليتم عرضه عند حفظ بيانات العرض إلى بعض صيغ [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/).

```csharp
public enum Shape
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | يشير إلى الشكل None. |
| VerticalLine | `1` | يشير إلى شكل الخط العمودي. |
| Pentagon | `2` | يشير إلى شكل الخماسي. |
| Triangle | `3` | يشير إلى شكل المثلث. |
| LeftBracket | `4` | يشير إلى شكل القوس الأيسر. |
| RightBracket | `5` | يشير إلى شكل القوس الأيمن. |
| ArrowDown | `6` | يشير إلى شكل السهم للأسفل. |
| LeftFade | `7` | يشير إلى شكل التلاشي الأيسر. |
| RightFade | `8` | يشير إلى شكل التلاشي الأيمن. |
| Diamond | `9` | يشير إلى شكل الماس. |
| Circle | `10` | يشير إلى شكل الدائرة. |

## الأمثلة

يعرض كيفية استخدام أنماط الشريط المخصصة.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    BarStyles = new List<BarStyle>()
};

// أضف نمط شريط لمهام الإنجاز
var style = new BarStyle();
// تعيين <see cref=\"T:Aspose.Tasks.Visualization.BarItemType\" /> لنمط الشريط
style.ItemType = BarItemType.Milestone;
// تعيين <see cref=\"T:System.Drawing.Color\" /> لنمط الشريط.
style.BarColor = Color.Green;
// تعيين <see cref=\"P:Aspose.Tasks.Visualization.BarStyle.BarShape\" /> لنمط الشريط
style.BarShape = BarShape.HalfHeight;
// تعيين <see cref="T:Aspose.Tasks.Visualization.Shape" /> في بداية الشريط
style.StartShape = Shape.LeftBracket;
// تعيين <see cref="T:System.Drawing.Color" /> للشكل في بداية الشريط
style.StartShapeColor = Color.Aqua;
// تعيين <see cref="T:Aspose.Tasks.Visualization.Shape" /> في نهاية الشريط
style.EndShape = Shape.RightBracket;
// تعيين <see cref="T:System.Drawing.Color" /> للشكل في نهاية الشريط
style.EndShapeColor = Color.Aquamarine;
// تعيين النص المراد عرضه على يمين الشريط.
style.TextStyle = new TextStyle();
style.TextStyle.BackgroundColor = Color.Black;

// هناك ميزة تسمح بتحويل نص الشريط
// لنقم بتعيين المحول للحصول على نص الشريط للعرض.
style.LeftBarTextConverter = task =>
{
    if (!task.Get(Tsk.Name).StartsWith("T"))
    {
        task.Set(Tsk.Name, "T" + task.Get(Tsk.Name));
    }

    return task.Get(Tsk.Name);
};

options.BarStyles.Add(style);

// احفظ المشروع
project.Save(OutDir + "WorkWithBarStyle_out.mpp", options);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


