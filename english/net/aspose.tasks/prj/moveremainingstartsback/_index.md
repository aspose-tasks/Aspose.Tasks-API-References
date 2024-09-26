---
title: Prj.MoveRemainingStartsBack
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether the beginning of remaining portions of tasks scheduled to start after the status date but started earlier should be moved back to the status date
type: docs
weight: 510
url: /net/aspose.tasks/prj/moveremainingstartsback/
---
## Prj.MoveRemainingStartsBack field

Determines whether the beginning of remaining portions of tasks scheduled to start after the status date but started earlier should be moved back to the status date.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsBack;
```

## Examples

Shows how to read/write Prj.MoveRemainingStartsBack property.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsBack, true);

Console.WriteLine("Move Remaining Starts Back: " + project.Get(Prj.MoveRemainingStartsBack));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


