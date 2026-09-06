---
title: "فئة BarStyle"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.Visualization.BarStyle فئة. غير النمط البصري للشريط للعنصر في عرض المشروع"
type: docs
weight: 2960
url: /ar/net/aspose.tasks.visualization/barstyle/
---
## BarStyle class

غيّر النمط البصري للبار للعنصر في عرض المشروع.

```csharp
public class BarStyle
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [BarStyle](barstyle/)() | ينشئ مثيلاً جديداً من الفئة `BarStyle`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BarColor](../../aspose.tasks.visualization/barstyle/barcolor/) { get; set; } | يحصل أو يعيّن اللون لنمط الشريط. |
| [BarShape](../../aspose.tasks.visualization/barstyle/barshape/) { get; set; } | يحصل أو يعيّن [`BarShape`](./barshape/) لنمط الشريط. |
| [BottomBarTextConverter](../../aspose.tasks.visualization/barstyle/bottombartextconverter/) { get; set; } | يحصل أو يعيّن محولًا معرفًا من قبل المستخدم للحصول على النص لتصميمه في أسفل شريط المهمة. يتجاوز قيمة الخاصية [`BottomField`](./bottomfield/). |
| [BottomField](../../aspose.tasks.visualization/barstyle/bottomfield/) { get; set; } | يحصل أو يعيّن حقلًا ليُعرض في أسفل الشريط. |
| [EndShape](../../aspose.tasks.visualization/barstyle/endshape/) { get; set; } | يحصل أو يعيّن [`Shape`](../shape/) في نهاية الشريط. |
| [EndShapeColor](../../aspose.tasks.visualization/barstyle/endshapecolor/) { get; set; } | يحصل أو يعيّن لون الشكل في نهاية الشريط. |
| [EndShapeType](../../aspose.tasks.visualization/barstyle/endshapetype/) { get; set; } | يحصل أو يعيّن نوع الشكل النهائي. [`GanttBarType`](../ganttbartype/). |
| [From](../../aspose.tasks.visualization/barstyle/from/) { get; set; } | يحصل أو يعيّن موضع نقطة البداية لشريط جانت. [`Field`](../../aspose.tasks/field/). |
| [InsideBarTextConverter](../../aspose.tasks.visualization/barstyle/insidebartextconverter/) { get; set; } | يحصل أو يعيّن محولًا معرفًا من قبل المستخدم للحصول على النص لتصميمه داخل شريط المهمة. يتجاوز قيمة الخاصية [`InsideField`](./insidefield/). |
| [InsideField](../../aspose.tasks.visualization/barstyle/insidefield/) { get; set; } | يحصل أو يعيّن حقلًا ليُعرض داخل الشريط. |
| [ItemType](../../aspose.tasks.visualization/barstyle/itemtype/) { get; set; } | يحصل أو يعيّن [`BarItemType`](../baritemtype/) لنمط الشريط. |
| [LeftBarTextConverter](../../aspose.tasks.visualization/barstyle/leftbartextconverter/) { get; set; } | يحصل أو يعيّن محولًا معرفًا من قبل المستخدم للحصول على النص ليُعرض على يسار شريط المهمة. يتجاوز قيمة الخاصية [`LeftField`](./leftfield/). |
| [LeftField](../../aspose.tasks.visualization/barstyle/leftfield/) { get; set; } | يحصل أو يعيّن حقلًا ليُعرض على يسار الشريط. |
| [RightBarTextConverter](../../aspose.tasks.visualization/barstyle/rightbartextconverter/) { get; set; } | يحصل أو يعيّن محولًا معرفًا من قبل المستخدم للحصول على النص لتصميمه على يمين شريط المهمة. يتجاوز قيمة الخاصية [`RightField`](./rightfield/). |
| [RightField](../../aspose.tasks.visualization/barstyle/rightfield/) { get; set; } | يحصل أو يضبط حقلًا ليتم عرضه على يمين الشريط. |
| [StartShape](../../aspose.tasks.visualization/barstyle/startshape/) { get; set; } | يحصل أو يضبط [`Shape`](../shape/) في بداية الشريط. |
| [StartShapeColor](../../aspose.tasks.visualization/barstyle/startshapecolor/) { get; set; } | يحصل أو يضبط لون الشكل في بداية الشريط. |
| [StartShapeType](../../aspose.tasks.visualization/barstyle/startshapetype/) { get; set; } | يحصل أو يعيّن نوع الشكل الابتدائي. |
| [TextStyle](../../aspose.tasks.visualization/barstyle/textstyle/) { get; set; } | يحصل أو يضبط نمط نص الشريط. |
| [To](../../aspose.tasks.visualization/barstyle/to/) { get; set; } | يحصل أو يعيّن موضع نقطة النهاية لشريط جانت. |
| [TopBarTextConverter](../../aspose.tasks.visualization/barstyle/topbartextconverter/) { get; set; } | يحصل أو يعيّن محولًا معرفًا من قبل المستخدم للحصول على النص لتصميمه في أعلى شريط المهمة. يتجاوز قيمة الخاصية [`TopField`](./topfield/). |
| [TopField](../../aspose.tasks.visualization/barstyle/topfield/) { get; set; } | يحصل أو يضبط حقلًا ليتم عرضه في أعلى الشريط. |

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


