---
title: "Asn.RateScale"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. وحدة الوقت لمعدل استخدام تعيين المورد المادي. يُعيد 0 إذا لم يُحدَّد"
type: docs
weight: 410
url: /ar/net/aspose.tasks/asn/ratescale/
---
## Asn.RateScale field

وحدة الوقت لمعدل استخدام تعيين المورد المادي. تُعيد 0 إذا لم يتم تعريفها.

```csharp
public static readonly Key<RateScaleType, AsnKey> RateScale;
```

## الأمثلة

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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateScaleType](../../ratescaletype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


