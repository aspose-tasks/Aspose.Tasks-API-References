---
title: Prj.MoveRemainingStartsForward
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether the beginning of remaining portions of tasks scheduled to have begun later should be moved up to the status date
type: docs
weight: 520
url: /net/aspose.tasks/prj/moveremainingstartsforward/
---
## Prj.MoveRemainingStartsForward field

Determines whether the beginning of remaining portions of tasks scheduled to have begun later should be moved up to the status date.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsForward;
```

## Examples

Shows how to read/write Prj.MoveRemainingStartsForward property.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsForward, true);

Console.WriteLine("Move Remaining Starts Forward: " + project.Get(Prj.MoveRemainingStartsForward));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


