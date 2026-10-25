---
title: "الفئة PrimaveraReadOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.PrimaveraReadOptions. تسمح بتحديد خيارات إضافية عند قراءة ملفات Primavera Xml أو Primavera Xer."
type: docs
weight: 1370
url: /ar/net/aspose.tasks/primaverareadoptions/
---
## PrimaveraReadOptions class

يسمح بتحديد خيارات إضافية عند قراءة ملفات Primavera Xml أو Primavera Xer.

```csharp
public class PrimaveraReadOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PrimaveraReadOptions](primaverareadoptions/)() | ينشئ مثيلًا جديدًا للفئة `PrimaveraReadOptions`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [PreserveUids](../../aspose.tasks/primaverareadoptions/preserveuids/) { get; set; } | يحصل أو يضبط علامة تحدد ما إذا كان يجب الحفاظ على المعرفات الفريدة الأصلية للكيانات. |
| [ProjectUid](../../aspose.tasks/primaverareadoptions/projectuid/) { get; set; } | يحصل أو يضبط معرف UID لمشروع يُقرأ من ملف يحتوي على مشاريع متعددة. |
| [ReadBaselineProjects](../../aspose.tasks/primaverareadoptions/readbaselineprojects/) { get; set; } | يحصل أو يضبط علامة تحدد ما إذا كان يجب تحميل مشاريع الخط الأساسي. القيمة الافتراضية هي true. |
| [UndefinedConstraintHandlingBehavior](../../aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/) { get; set; } | يحدد السلوك المستخدم لمعالجة المهام ذات القيود غير المعرفة المقروءة من تنسيق XER. |

## الأمثلة

يظهر كيفية قراءة مشروع من ملف Primavera XML أو Primavera XER يحتوي على مشاريع متعددة.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// يعيد مشروعًا بمعرف UID خاص.
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


