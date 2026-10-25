---
title: "VbaReference.Equals"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة VbaReference. تُعيد قيمة تشير إلى ما إذا كانت هذه المثيلة مساوية للكيان VbaReference المحدد"
type: docs
weight: 40
url: /ar/net/aspose.tasks/vbareference/equals/
---
## Equals(VbaReference) {#equals}

تُعيد قيمة تشير إلى ما إذا كانت هذه المثيلة مساوية للكيان [`VbaReference`](../) المحدد.

```csharp
public bool Equals(VbaReference other)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| other | VbaReference | الكائن [`VbaReference`](../) المحدد للمقارنة مع هذه المثيلة. |

### قيمة الإرجاع

تُعيد true إذا كانت هذه المثيلة مساوية للكيان [`VbaReference`](../) المحدد؛ وإلا، false.

## الأمثلة

يوضح كيفية فحص مساواة مرجع VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// يتم فحص مساواة المراجع مقابل اسم المرجع.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### انظر أيضًا

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

تُعيد قيمة تشير إلى ما إذا كانت هذه المثيلة مساوية للكيان [`VbaReference`](../) المحدد.

```csharp
public override bool Equals(object obj)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| obj | Object | الكائن [`VbaReference`](../) المحدد للمقارنة مع هذه المثيلة. |

### قيمة الإرجاع

تُعيد true إذا كانت هذه المثيلة مساوية للكيان [`VbaReference`](../) المحدد؛ وإلا، false.

## الأمثلة

يوضح كيفية فحص مساواة مرجع VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// يتم فحص مساواة المراجع مقابل اسم المرجع.
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### انظر أيضًا

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


