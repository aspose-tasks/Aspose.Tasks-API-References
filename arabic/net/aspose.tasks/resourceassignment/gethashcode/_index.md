---
title: "ResourceAssignment.GetHashCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceAssignment. تُرجع قيمة hash code للنسخة من فئة ResourceAssignment"
type: docs
weight: 710
url: /ar/net/aspose.tasks/resourceassignment/gethashcode/
---
## ResourceAssignment.GetHashCode method

تُرجع قيمة hash code للنسخة من فئة [`ResourceAssignment`](../).

```csharp
public override int GetHashCode()
```

### قيمة الإرجاع

تُرجع قيمة رمز تجزئة لهذا الكائن.

## الأمثلة

يظهر كيفية الحصول على hash code لتعيين مورد.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(2);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(3);

// اطبع hash codes للتعيين
Console.WriteLine("Resource Assignment 1 Hash Code: {0}", resourceAssignment1.GetHashCode());
Console.WriteLine("Resource Assignment 2 Hash Code: {0}", resourceAssignment2.GetHashCode());
```

### انظر أيضًا

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


