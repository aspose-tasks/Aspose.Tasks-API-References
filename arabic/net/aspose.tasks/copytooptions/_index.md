---
title: "الفئة CopyToOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.CopyToOptions. تسمح بتحديد خيارات إضافية عند نسخ بيانات المشروع"
type: docs
weight: 340
url: /ar/net/aspose.tasks/copytooptions/
---
## CopyToOptions class

يسمح بتحديد خيارات إضافية عند نسخ بيانات المشروع.

```csharp
public class CopyToOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [CopyToOptions](copytooptions/)() | ينشئ مثيلاً جديداً للفئة `CopyToOptions`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CopyViewData](../../aspose.tasks/copytooptions/copyviewdata/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب نسخ بيانات العرض أثناء نسخ بيانات المشروع. القيمة الافتراضية هي true. |

## الأمثلة

يظهر كيفية استخدام خيارات نسخ المشروع.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// تخطي نسخ بيانات العرض أثناء نسخ بيانات المشروع العامة.
var copyToOptions = new CopyToOptions();
copyToOptions.CopyViewData = false;
project.CopyTo(mppProject, copyToOptions);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


