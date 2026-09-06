---
title: "MPPSaveOptions.WriteViewData"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية MPPSaveOptions. تحصل أو تعين قيمة تشير إلى ما إذا كان يجب كتابة بيانات العرض عند حفظ مشروع بتنسيق MPP. تشمل بيانات العرض مجموعات Project.Views Filters و Tables."
type: docs
weight: 80
url: /ar/net/aspose.tasks.saving/mppsaveoptions/writeviewdata/
---
## MPPSaveOptions.WriteViewData property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب كتابة بيانات العرض عند حفظ المشروع إلى تنسيق MPP. تشمل بيانات العرض مجموعات Project.Views و Filters و Tables.

```csharp
public bool WriteViewData { get; set; }
```

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

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


