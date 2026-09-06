---
title: "PrimaveraSaveOptions.RenumberActivityIds"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PrimaveraSaveOptions. يحصل أو يحدد قيمة تشير إلى ما إذا كان هناك حاجة لإعادة ترقيم معرفات الأنشطة"
type: docs
weight: 50
url: /ar/net/aspose.tasks.saving/primaverasaveoptions/renumberactivityids/
---
## PrimaveraSaveOptions.RenumberActivityIds property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان هناك حاجة لإعادة ترقيم معرفات الأنشطة.

```csharp
public bool RenumberActivityIds { get; set; }
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


