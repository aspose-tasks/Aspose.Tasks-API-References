---
title: "الفئة View"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.View. تمثل عرضًا في Project"
type: docs
weight: 2890
url: /ar/net/aspose.tasks/view/
---
## View class

يمثل عرضًا في Project.

```csharp
public class View : IComparable<View>
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [View](view/#constructor)() | يُنشئ مثيلًا جديدًا للفئة `View`. |
| [View](view/#constructor_1)(ViewScreen) | يُنشئ مثيلًا جديدًا للفئة `View`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | يحصل أو يضبط مرشحًا يُستخدم في عرض واحد. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | يحصل أو يضبط مجموعة من العرض الواحد. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان Microsoft Project يبرز الفلتر للعرض الواحد. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | يحصل أو يضبط اسم كائن View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | يحصل على مثيل من الفئة [`PageInfo`](./pageinfo/). تمثل بيانات إعداد الصفحة الموجودة في تنسيق ملف mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | يحصل على الأصل لكائن View. للقراءة فقط [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | يحصل على نوع الشاشة للعرض الواحد. للقراءة فقط [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان Microsoft Project يعرض اسم العرض الواحد في قائمة العرض أو قوائم العروض الأخرى المنسدلة في الشريط. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | يحصل أو يضبط جدولًا للعرض الواحد. |
| [Type](../../aspose.tasks/view/type/) { get; } | يحصل على نوع العنصر في العرض الواحد، مثل المهام أو الموارد. للقراءة فقط [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | يحصل على المعرف الفريد للعرض. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | يحصل على مجموعة من الكائنات التي تمثل موضع ومظهر [`OleObject`](../oleobject/) في العرض. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | يقارن النسخة الحالية مع كائن آخر من نفس النوع ويعيد عددًا صحيحًا يشير إلى ما إذا كانت النسخة الحالية تسبق أو تلي أو تقع في نفس الموضع في ترتيب الفرز كما الكائن الآخر. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | يعيد قيمة رمز تجزئة للنسخة من الفئة [`Resource`](../resource/). |
| [operator ==](../../aspose.tasks/view/op_equality/) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [operator &gt;](../../aspose.tasks/view/op_greaterthan/) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أكبر من كائن محدد. |
| [operator &gt;=](../../aspose.tasks/view/op_greaterthanorequal/) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أكبر من أو مساوية لكائن محدد. |
| [operator !=](../../aspose.tasks/view/op_inequality/) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة غير مساوية لكائن محدد. |
| [operator &lt;](../../aspose.tasks/view/op_lessthan/) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أصغر من كائن محدد. |
| [operator &lt;=](../../aspose.tasks/view/op_lessthanorequal/) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أصغر من أو مساوية لكائن محدد. |

## الأمثلة

يوضح كيفية العمل مع عرض Project وإضافة عمود إلى العرض الافتراضي (الذي يُظهر عندما يُفتح ملف MPP في MS Project).

```csharp
// إنشاء مشروع فارغ بدون عروض
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// تعديل العرض الافتراضي (إنه عرض مخطط جانت).
// أو يمكنك اختيار العرض بالاسم أو عبر شاشة العرض باستخدام مجموعة project.View.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// يجب استخدام علم WriteViewData لحفظ تعديلات خصائص العرض.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

يعرض كيفية العمل مع عروض MS Project.

```csharp
// إنشاء مشروع فارغ بدون عروض
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// إنشاء عرض مخطط جانت قياسي
View view = new GanttChartView();

// تعيين بعض خصائص العرض
// تعيين قيمة تشير إلى ما إذا كان Microsoft Project يعرض اسم العرض الفردي في القائمة المنسدلة View أو Other Views في الشريط.
view.ShowInMenu = true;
// تعيين قيمة تشير إلى ما إذا كان Microsoft Project يبرز الفلتر لعرض واحد.
view.HighlightFilter = true;

// كتابة الخصائص التالية غير مدعومة
// يضبط الفلتر المستخدم في عرض واحد
view.Filter = null;
// يضبط مجموعة العرض الفردي
view.Group = null;
// يضبط جدول العرض الفردي
view.Table = null;

// لنضبط بعض إعدادات العرض
// تعيين عدد الأعمدة الأولى التي سيتم طباعتها على جميع الصفحات
view.PageInfo.PageViewSettings.FirstColumnsCount = 4;
// تعيين قيمة تشير إلى ما إذا كان يجب طباعة عدد محدد من الأعمدة الأولى على جميع الصفحات
view.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

// إضافة العرض إلى مشروعنا
project.Views.Add(view);

// يجب استخدام علامة WriteViewData لحفظ تعديلات project.Views.
project.Save(OutDir + "WorkWithView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
// لنفحص بعض خصائص العرض المضاف حديثًا
// اطبع المعرف الفريد لعرض
Console.WriteLine("View Uid: " + view.Uid);
// اطبع نوع الشاشة للعرض الفردي
Console.WriteLine("View Screen: " + view.Screen);
Console.WriteLine("View Type: " + view.Type);
Console.WriteLine("Parent Project of the view: " + view.ParentProject.Get(Prj.Name));
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


