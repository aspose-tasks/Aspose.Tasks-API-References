---
title: "View.Group"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية View. تحصل أو تعيّن مجموعة من العرض الفردي"
type: docs
weight: 30
url: /ar/net/aspose.tasks/view/group/
---
## View.Group property

يحصل أو يضبط مجموعة من العرض الواحد.

```csharp
public Group Group { get; set; }
```

## الأمثلة

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

* class [Group](../../group/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


