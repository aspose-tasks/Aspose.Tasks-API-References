---
title: "VbaModuleAttribute.Equals"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة VbaModuleAttribute. تُرجع قيمة تُشير إلى ما إذا كانت هذه الحالة مساوية لكائن VbaModuleAttribute المحدد"
type: docs
weight: 30
url: /ar/net/aspose.tasks/vbamoduleattribute/equals/
---
## Equals(VbaModuleAttribute) {#equals}

تُرجع قيمة تُشير إلى ما إذا كانت هذه الحالة مساوية لكائن [`VbaModuleAttribute`](../) المحدد.

```csharp
public bool Equals(VbaModuleAttribute other)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| other | VbaModuleAttribute | الكائن [`VbaModuleAttribute`](../) المحدد للمقارنة مع هذه الحالة. |

### قيمة الإرجاع

تُرجع true إذا كانت هذه الحالة مساوية للكائن [`VbaModuleAttribute`](../) المحدد؛ وإلا، false.

## الأمثلة

يُظهر كيفية التحقق من مساواة سمات وحدة VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### انظر أيضًا

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

تُرجع قيمة تُشير إلى ما إذا كانت هذه الحالة مساوية لكائن [`VbaModuleAttribute`](../) المحدد.

```csharp
public override bool Equals(object obj)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| obj | Object | الكائن [`VbaModuleAttribute`](../) المحدد للمقارنة مع هذه الحالة. |

### قيمة الإرجاع

تُرجع true إذا كانت هذه الحالة مساوية للكائن [`VbaModuleAttribute`](../) المحدد؛ وإلا، false.

## الأمثلة

يُظهر كيفية التحقق من مساواة سمات وحدة VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### انظر أيضًا

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


