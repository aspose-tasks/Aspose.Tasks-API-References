---
title: "VbaModuleAttribute.GetHashCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة VbaModuleAttribute. تُرجع قيمة رمز تجزئة لهذا VbaModuleAttribute"
type: docs
weight: 40
url: /ar/net/aspose.tasks/vbamoduleattribute/gethashcode/
---
## VbaModuleAttribute.GetHashCode method

تُرجع قيمة رمز تجزئة لهذا [`VbaModuleAttribute`](../).

```csharp
public override int GetHashCode()
```

### قيمة الإرجاع

يعيد قيمة رمز التجزئة لهذا الكائن.

## الأمثلة

يُظهر كيفية الحصول على رمز تجزئة لسمة وحدة VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];

// طباعة رموز التجزئة لسمة وحدة VBA
Console.WriteLine("Hash codes of VBA module attributes are based on key and value hash codes.");
Console.WriteLine("VBA module attribute 1 Hash Code: {0}", attribute1.GetHashCode());
Console.WriteLine("VBA module attribute 2 Hash Code: {0}", attribute2.GetHashCode());
```

### انظر أيضًا

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


