---
title: Prj.EarnedValueMethod
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The default method for calculating earned value
type: docs
weight: 310
url: /net/aspose.tasks/prj/earnedvaluemethod/
---
## Prj.EarnedValueMethod field

The default method for calculating earned value.

```csharp
public static readonly Key<EarnedValueMethodType, PrjKey> EarnedValueMethod;
```

## Examples

Shows how to read/write Prj.EarnedValueMethod property.

```csharp
var project = new Project();

project.Set(Prj.EarnedValueMethod, EarnedValueMethodType.PhysicalPercentComplete);

Console.WriteLine("Earned Value Method: " + project.Get(Prj.EarnedValueMethod));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


