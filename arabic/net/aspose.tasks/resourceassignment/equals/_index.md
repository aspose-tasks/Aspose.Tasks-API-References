---
title: "ResourceAssignment.Equals"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceAssignment. تُرجع قيمة تشير إلى ما إذا كان هذا المثيل مساويًا لمثيل محدد من فئة ResourceAssignment"
type: docs
weight: 690
url: /ar/net/aspose.tasks/resourceassignment/equals/
---
## Equals(ResourceAssignment) {#equals}

تُرجع قيمة تشير إلى ما إذا كان هذا المثيل مساويًا لمثيل محدد من فئة [`ResourceAssignment`](../).

```csharp
public bool Equals(ResourceAssignment other)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| other | ResourceAssignment | المثيل المحدد من فئة [`ResourceAssignment`](../) للمقارنة مع هذا المثيل. |

### قيمة الإرجاع

**True** if the specified instance of the [`ResourceAssignment`](../) class has the same UID value as this instance; otherwise, **false**.

## الأمثلة

يظهر كيفية التحقق من مساواة تعيين المورد.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### انظر أيضًا

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

```csharp
public override bool Equals(object obj)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| obj | كائن | الكائن للمقارنة مع هذه المثيلة. |

### قيمة الإرجاع

**True** if o is a ResourceAssignment that assign the same resource and task as this instance; otherwise, **false**.

## الأمثلة

يظهر كيفية التحقق من مساواة تعيين المورد.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### انظر أيضًا

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


