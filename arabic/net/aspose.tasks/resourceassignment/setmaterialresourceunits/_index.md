---
title: "ResourceAssignment.SetMaterialResourceUnits"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceAssignment. تعين الوحدات لتعيين مورد مادي مع استهلاك مادي متغير. يعني الاستهلاك المادي المتغير أنه كلما تغيرت مدة التعيين يتغير كمية المواد المستخدمة بشكل متناسب"
type: docs
weight: 760
url: /ar/net/aspose.tasks/resourceassignment/setmaterialresourceunits/
---
## ResourceAssignment.SetMaterialResourceUnits method

يعيّن الوحدات لتعيين مورد مادي باستهلاك مادي متغيّر. يعني الاستهلاك المادي المتغيّر أنه كلما تغيرت مدة التعيين، تتغير كمية المواد المستخدمة بشكل متناسب.

```csharp
public void SetMaterialResourceUnits(double units, RateScaleType rateScaleType)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| الوحدات | Double | عدد الوحدات المتراكمة خلال الفترة الزمنية. |
| rateScaleType | RateScaleType | الفترة الزمنية التي تُتراكم فيها قيمة الوحدة. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | إذا تم استدعاء الطريقة لتعيين مورد غير مادي. |

## ملاحظات

على سبيل المثال، لتعيين '123/شهر'، يجب استدعاء SetUnitsScaled(123D, RateScaleType.Month).

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

### انظر أيضًا

* enum [RateScaleType](../../ratescaletype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


