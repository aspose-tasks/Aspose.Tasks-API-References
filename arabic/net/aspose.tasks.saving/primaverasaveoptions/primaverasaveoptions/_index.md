---
title: "PrimaveraSaveOptions.PrimaveraSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ PrimaveraSaveOptions. يهيئ نسخة جديدة من فئة PrimaveraSaveOptions"
type: docs
weight: 10
url: /ar/net/aspose.tasks.saving/primaverasaveoptions/primaverasaveoptions/
---
## PrimaveraSaveOptions constructor

يهيئ نسخة جديدة من الفئة [`PrimaveraSaveOptions`](../).

```csharp
public PrimaveraSaveOptions()
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


