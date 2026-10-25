---
title: "تعداد ViewScreen"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.ViewScreen. يحدد نوع الشاشة للعرض"
type: docs
weight: 2910
url: /ar/net/aspose.tasks/viewscreen/
---
## ViewScreen enumeration

يحدد نوع الشاشة للعرض.

```csharp
public enum ViewScreen
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Calendar | `13` | عرض التقويم. |
| Gantt | `1` | عرض جانت. |
| NetworkDiagram | `2` | عرض مخطط الشبكة. |
| RelationshipDiagram | `3` | عرض مخطط العلاقة. |
| ResourceForm | `6` | عرض نموذج المورد. |
| ResourceGraph | `8` | عرض مخطط المورد. |
| ResourceNameForm | `12` | عرض نموذج اسم المورد. |
| ResourceSheet | `7` | عرض ورقة المورد. |
| ResourceUsage | `15` | عرض استخدام المورد. |
| TaskDetailsForm | `10` | عرض نموذج تفاصيل المهمة. |
| TaskForm | `4` | عرض نموذج المهمة. |
| TaskNameForm | `11` | عرض نموذج اسم المهمة. |
| TaskSheet | `5` | عرض ورقة المهمة. |
| TaskUsage | `14` | عرض استخدام المهمة. |

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


