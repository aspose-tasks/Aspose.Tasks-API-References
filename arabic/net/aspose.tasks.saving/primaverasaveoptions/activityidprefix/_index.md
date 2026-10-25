---
title: "PrimaveraSaveOptions.ActivityIdPrefix"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PrimaveraSaveOptions. يحصل أو يحدد البادئة المستخدمة في إعادة ترقيم معرفات الأنشطة"
type: docs
weight: 30
url: /ar/net/aspose.tasks.saving/primaverasaveoptions/activityidprefix/
---
## PrimaveraSaveOptions.ActivityIdPrefix property

يحصل أو يعيّن البادئة المستخدمة في إعادة ترقيم معرفات الأنشطة.

```csharp
public string ActivityIdPrefix { get; set; }
```

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

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


