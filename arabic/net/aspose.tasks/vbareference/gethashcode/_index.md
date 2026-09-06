---
title: "VbaReference.GetHashCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة VbaReference. تُعيد قيمة تجزئة لهذا VbaReference"
type: docs
weight: 50
url: /ar/net/aspose.tasks/vbareference/gethashcode/
---
## VbaReference.GetHashCode method

تُعيد قيمة تجزئة لهذا [`VbaReference`](../).

```csharp
public override int GetHashCode()
```

### قيمة الإرجاع

يعيد قيمة رمز التجزئة لهذا الكائن.

## الأمثلة

يوضح كيفية الحصول على قيمة تجزئة لمرجع VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// قيمة التجزئة للمرجع هي قيمة تجزئة معرف GUID الداخلي للمرجع
Console.WriteLine("VBA reference Hash Code: {0}", reference1.GetHashCode());
Console.WriteLine("VBA reference Hash Code: {0}", reference2.GetHashCode());
```

### انظر أيضًا

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


