---
title: "فئة VbaModuleAttribute"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.VbaModuleAttribute. السمة لكائن VbaModule."
type: docs
weight: 2820
url: /ar/net/aspose.tasks/vbamoduleattribute/
---
## VbaModuleAttribute class

السمة لكائن [`VbaModule`](../vbamodule/).

```csharp
public sealed class VbaModuleAttribute : IEquatable<VbaModuleAttribute>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Key](../../aspose.tasks/vbamoduleattribute/key/) { get; } | يحصل أو يعيّن المفتاح لسمة وحدة VBA. |
| [Value](../../aspose.tasks/vbamoduleattribute/value/) { get; } | يحصل أو يعيّن القيمة لسمة وحدة VBA. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals_1)(object) | يعيد قيمة تشير إلى ما إذا كانت هذه المثيلة مساوية لكائن `VbaModuleAttribute` المحدد. |
| [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals)(VbaModuleAttribute) | يعيد قيمة تشير إلى ما إذا كانت هذه المثيلة مساوية لكائن `VbaModuleAttribute` المحدد. |
| override [GetHashCode](../../aspose.tasks/vbamoduleattribute/gethashcode/)() | يعيد قيمة تجزئة (hash code) لهذا `VbaModuleAttribute`. |

## الأمثلة

يظهر كيفية العمل مع سمات وحدة VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("  VB Name: " + attribute.Key);
        Console.WriteLine("  Module: " + attribute.Value);
    }
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


