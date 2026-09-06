---
title: "MPPSaveOptions.RemoveInvalidAssignments"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية MPPSaveOptions. تحصل أو تعين قيمة تشير إلى ما إذا كان يجب إزالة تعيينات الموارد غير الصالحة عند الحفظ إلى MPP. يقوم MS Project بإنشاء تعيين مورد فارغ لكل مهمة. اضبط هذه العلامة على true لإزالتها عند الحفظ."
type: docs
weight: 40
url: /ar/net/aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/
---
## MPPSaveOptions.RemoveInvalidAssignments property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إزالة تعيينات الموارد غير الصالحة عند الحفظ إلى MPP. يقوم MS Project بإنشاء تعيين مورد فارغ لكل مهمة. اضبط هذا العلم على true لإزالتها عند الحفظ.

```csharp
public bool RemoveInvalidAssignments { get; set; }
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


