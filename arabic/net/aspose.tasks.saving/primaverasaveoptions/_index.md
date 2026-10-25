---
title: "فئة PrimaveraSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Saving.PrimaveraSaveOptions. تسمح بتحديد خيارات إضافية عند حفظ المشروع بتنسيق Primavera XER."
type: docs
weight: 2150
url: /ar/net/aspose.tasks.saving/primaverasaveoptions/
---
## PrimaveraSaveOptions class

يسمح بتحديد خيارات إضافية عند حفظ المشروع إلى تنسيق Primavera XER.

```csharp
public class PrimaveraSaveOptions : SimpleSaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PrimaveraSaveOptions](primaverasaveoptions/)() | يُنشئ مثيلًا جديدًا من الفئة `PrimaveraSaveOptions`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ActivityIdIncrement](../../aspose.tasks.saving/primaverasaveoptions/activityidincrement/) { get; set; } | يحصل أو يعيّن الزيادة المستخدمة في إعادة ترقيم معرفات الأنشطة. |
| [ActivityIdPrefix](../../aspose.tasks.saving/primaverasaveoptions/activityidprefix/) { get; set; } | يحصل أو يعيّن البادئة المستخدمة في إعادة ترقيم معرفات الأنشطة. |
| [ActivityIdSuffix](../../aspose.tasks.saving/primaverasaveoptions/activityidsuffix/) { get; set; } | يحصل أو يعيّن اللاحقة المستخدمة في إعادة ترقيم معرفات الأنشطة. |
| [RenumberActivityIds](../../aspose.tasks.saving/primaverasaveoptions/renumberactivityids/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان هناك حاجة لإعادة ترقيم معرفات الأنشطة. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | يحصل أو يعيّن التنسيق الذي سيتم حفظ المستند به إذا تم استخدام كائن خيارات الحفظ هذا. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تخطي تعيينات الموارد إلى المهام الملخصة أثناء التصدير. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | يحصل أو يعيّن المقارن لفرز المهام على مخطط جانت ومخطط ورقة المهام. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | يحصل أو يعيّن الشرط المستخدم لتصفية المهام المعروضة على مخططات جانت، ورقة المهام، واستخدام المهام. |

## الأمثلة

يعرض كيفية العمل مع <see cref=\"Aspose.Tasks.Saving.PrimaveraSaveOptions\" />.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// إنشاء خيارات حفظ Primavera وضبطها
var options = new PrimaveraSaveOptions
                  {
                      // تحديد البادئة واللاحقة لنشاط
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // التحكم في إعادة ترقيم الأنشطة
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### انظر أيضًا

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


