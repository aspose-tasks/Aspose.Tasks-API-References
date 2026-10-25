---
title: "Project.DefaultView"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. تحصل أو تعين العرض الافتراضي للمشروع"
type: docs
weight: 360
url: /ar/net/aspose.tasks/project/defaultview/
---
## Project.DefaultView property

يحصل أو يعيّن العرض الافتراضي للمشروع.

```csharp
public View DefaultView { get; set; }
```

## الأمثلة

يظهر كيفية العمل مع العرض الافتراضي لمشروع.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// احصل على العرض الافتراضي
UsageView view = (TaskUsageView)project.DefaultView;

// عمود عنوان التفاصيل لن يتم عرضه
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// عرض عمود عنوان التفاصيل
view.DisplayDetailsHeaderColumn = true;

// تكرار عنوان التفاصيل على جميع صفوف التعيينات
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

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

### انظر أيضًا

* class [View](../../view/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


