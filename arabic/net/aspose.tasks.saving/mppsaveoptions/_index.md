---
title: "الفئة MPPSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Saving.MPPSaveOptions. تسمح بتحديد خيارات إضافية عند حفظ بيانات المشروع إلى MPP"
type: docs
weight: 2050
url: /ar/net/aspose.tasks.saving/mppsaveoptions/
---
## MPPSaveOptions class

يسمح بتحديد خيارات إضافية عند حفظ بيانات المشروع إلى MPP.

```csharp
public class MPPSaveOptions : SimpleSaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [MPPSaveOptions](mppsaveoptions/)() | يُنشئ مثيلاً جديدًا من الفئة `MPPSaveOptions`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ClearVba](../../aspose.tasks.saving/mppsaveoptions/clearvba/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إزالة بيانات ماكرو VBA الموجودة عند حفظ المشروع بتنسيق MPP. |
| [ProtectionPassword](../../aspose.tasks.saving/mppsaveoptions/protectionpassword/) { get; set; } | يحصل أو يعيّن كلمة مرور تُستخدم لحماية ملف MPP الناتج. حاليًا يتم دعم ذلك لتنسيقات MS Project 2010 وما بعدها. القيمة Null تشير إلى أن ملف المشروع غير محمي. |
| [RemoveInvalidAssignments](../../aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إزالة تعيينات الموارد غير الصالحة عند الحفظ إلى MPP. يقوم MS Project بإنشاء تعيين مورد فارغ لكل مهمة. اضبط هذا العلم على true لإزالتها عند الحفظ. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | يحصل أو يعيّن التنسيق الذي سيتم حفظ المستند به إذا تم استخدام كائن خيارات الحفظ هذا. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | يحصل أو يعيّن المقارن لفرز المهام على مخطط جانت ومخطط ورقة المهام. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | يحصل أو يعيّن الشرط المستخدم لتصفية المهام المعروضة على مخططات جانت، ورقة المهام، واستخدام المهام. |
| [WriteFilters](../../aspose.tasks.saving/mppsaveoptions/writefilters/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب كتابة بيانات الفلاتر عند حفظ المشروع إلى تنسيق MPP. تشمل بيانات الفلاتر مجموعات Project.TaskFilters و Project.ResourceFilters. |
| [WriteGroups](../../aspose.tasks.saving/mppsaveoptions/writegroups/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب كتابة بيانات المجموعات عند حفظ المشروع إلى تنسيق MPP. تشمل بيانات المجموعات مجموعات Project.TaskGroups و Project.ResourceGroups. |
| [WriteVba](../../aspose.tasks.saving/mppsaveoptions/writevba/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحديث بيانات ماكرو VBA الموجودة في ملف MPP. حاليًا يتم دعم كتابة VbaModule.SourceCode. |
| [WriteViewData](../../aspose.tasks.saving/mppsaveoptions/writeviewdata/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب كتابة بيانات العرض عند حفظ المشروع إلى تنسيق MPP. تشمل بيانات العرض مجموعات Project.Views و Filters و Tables. |

## الأمثلة

يوضح كيفية حفظ المشروع في تدفق كملف MPP.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

    // إنشاء خيارات الحفظ
    SimpleSaveOptions options = new MPPSaveOptions
    {
        // يعيّن قيمة تشير إلى ما إذا كان يجب إزالة تعيينات الموارد غير الصالحة عند الحفظ إلى MPP
        RemoveInvalidAssignments = true
    };

    // حفظ MPP باستخدام الخيارات
    project.Save(stream, options);
}
```

### انظر أيضًا

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


