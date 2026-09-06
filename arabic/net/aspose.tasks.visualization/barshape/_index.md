---
title: "تعداد BarShape"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.Visualization.BarShape تعداد. شكل مستطيل الشريط"
type: docs
weight: 2950
url: /ar/net/aspose.tasks.visualization/barshape/
---
## BarShape enumeration

شكل مستطيل الشريط.

```csharp
public enum BarShape
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Full | `0` | يشير إلى شكل شريط مستطيل كامل. |
| HalfHeight | `1` | يشير إلى شكل شريط مستطيل نصف الارتفاع محاذى إلى الأعلى. |
| HalfHeightBottom | `2` | يشير إلى شكل شريط مستطيل نصف الارتفاع محاذى إلى الأسفل. |
| Thin | `3` | يشير إلى شكل خط محاذى إلى الوسط. |
| None | `4` | يشير إلى شكل شريط لا شيء. |
| Middle | `5` | يشير إلى شكل خط محاذى إلى الوسط. |
| LineBottom | `6` | يشير إلى شكل خط محاذى إلى الأسفل. |
| LineTop | `7` | يشير إلى شكل خط محاذى إلى الأعلى. |

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


