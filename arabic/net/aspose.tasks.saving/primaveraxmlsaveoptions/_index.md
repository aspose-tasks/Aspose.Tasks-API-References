---
title: "الفئة PrimaveraXmlSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Saving.PrimaveraXmlSaveOptions. تسمح بتحديد خيارات إضافية عند حفظ المشروع إلى تنسيق XML الخاص بـ Primavera"
type: docs
weight: 2160
url: /ar/net/aspose.tasks.saving/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions class

يسمح بتحديد خيارات إضافية عند حفظ المشروع إلى تنسيق Primavera XML.

```csharp
public class PrimaveraXmlSaveOptions : SimpleSaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PrimaveraXmlSaveOptions](primaveraxmlsaveoptions/)() | يُنشئ مثيلًا جديدًا للفئة `PrimaveraXmlSaveOptions`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | يحصل أو يعيّن التنسيق الذي سيتم حفظ المستند به إذا تم استخدام كائن خيارات الحفظ هذا. |
| [SaveRootTask](../../aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان سيتم حفظ مهمة جذر أم لا. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تخطي تعيينات الموارد إلى المهام الملخصة أثناء التصدير. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | يحصل أو يعيّن المقارن لفرز المهام على مخطط جانت ومخطط ورقة المهام. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | يحصل أو يعيّن الشرط المستخدم لتصفية المهام المعروضة على مخططات جانت، ورقة المهام، واستخدام المهام. |

## الأمثلة

يظهر كيفية تصدير إلى ملف Primavera XML.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### انظر أيضًا

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


