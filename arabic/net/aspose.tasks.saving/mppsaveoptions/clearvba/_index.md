---
title: "MPPSaveOptions.ClearVba"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية MPPSaveOptions. تحصل أو تعين قيمة تشير إلى ما إذا كان يجب إزالة بيانات ماكرو VBA الموجودة عند حفظ مشروع بتنسيق MPP."
type: docs
weight: 20
url: /ar/net/aspose.tasks.saving/mppsaveoptions/clearvba/
---
## MPPSaveOptions.ClearVba property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إزالة بيانات ماكرو VBA الموجودة عند حفظ المشروع بتنسيق MPP.

```csharp
public bool ClearVba { get; set; }
```

## الأمثلة

يظهر كيفية إزالة ماكرو VBA من ملف MPP.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

### انظر أيضًا

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


