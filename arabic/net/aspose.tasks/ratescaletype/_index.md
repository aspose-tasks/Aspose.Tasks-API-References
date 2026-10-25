---
title: "تعداد RateScaleType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.RateScaleType. يحدد نوع مقياس المعدل"
type: docs
weight: 1650
url: /ar/net/aspose.tasks/ratescaletype/
---
## RateScaleType enumeration

يحدد نوع مقياس المعدل.

```csharp
public enum RateScaleType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `0` | يشير إلى نوع مقياس المعدل غير معرف. |
| Minute | `1` | يشير إلى نوع مقياس المعدل بالدقيقة. |
| Hour | `2` | يشير إلى نوع مقياس المعدل بالساعة. |
| Day | `3` | يشير إلى نوع مقياس المعدل باليوم. |
| Week | `4` | يشير إلى نوع مقياس المعدل بالأسبوع. |
| Month | `5` | يشير إلى نوع مقياس المعدل بالشهر. |
| Quarter | `6` | يشير إلى نوع مقياس المعدل بالربع. |
| Year | `7` | يشير إلى نوع مقياس المعدل بالسنة. |

## الأمثلة

يعرض كيفية تعيين استهلاك مادة متغير (مثال: '10/day' أو '1/week') لتخصيص مورد مادي.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// افترض أننا نريد تعيين استهلاك مادة '1/week'.
materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);
```

يعرض كيفية التعامل مع مقياس معدل التخصيص عندما نريد تعيين استهلاك مادة متغير (مثال: '10/day' أو '1/week') لتخصيص مورد مادي.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var nonMaterialResource = project.Resources.Add("nonMaterialResource");
nonMaterialResource.Set(Rsc.Type, ResourceType.Work);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// افترض أننا نريد تعيين استهلاك مادة '1/week'.
// يجب أن نعين المعدل الساعي إلى خاصية Units، لذا نقسم 1D على عدد الساعات في الأسبوع.
materialResourceAssignment.Set(Asn.Units, 1D / 40);
materialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

// يرجى ملاحظة أنه بدءًا من الإصدار 24.4 يمكن القيام بذلك عن طريق استدعاء طريقة واحدة:
// materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);

var nonMaterialResourceAssignment = project.ResourceAssignments.Add(task, nonMaterialResource);
nonMaterialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

project.Save(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp", SaveFileFormat.Mpp);

var resavedProject = new Project(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp");

var resavedMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(2);
Console.WriteLine(resavedMaterialResourceAssignment.Get(Asn.RateScale));

// يمكن فقط لتخصيصات الموارد المادية أن تحتوي على قيمة مقياس معدل غير صفرية.
var resavedNonMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(3);
Console.WriteLine(resavedNonMaterialResourceAssignment.Get(Asn.RateScale));
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


