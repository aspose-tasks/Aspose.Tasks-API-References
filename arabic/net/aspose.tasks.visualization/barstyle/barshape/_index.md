---
title: "BarStyle.BarShape"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية BarStyle. يحصل أو يضبط BarShape لنمط الشريط"
type: docs
weight: 30
url: /ar/net/aspose.tasks.visualization/barstyle/barshape/
---
## BarStyle.BarShape property

يحصل أو يضبط `BarShape` لنمط الشريط.

```csharp
public BarShape BarShape { get; set; }
```

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

* enum [BarShape](../../barshape/)
* class [BarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../barstyle/)
* assembly [Aspose.Tasks](../../../)


