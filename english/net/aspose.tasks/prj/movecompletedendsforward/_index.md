---
title: Prj.MoveCompletedEndsForward
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether the end of completed portions of tasks scheduled to have been completed before the status date but begun later should be moved up to the status date
type: docs
weight: 500
url: /net/aspose.tasks/prj/movecompletedendsforward/
---
## Prj.MoveCompletedEndsForward field

Determines whether the end of completed portions of tasks scheduled to have been completed before the status date but begun later should be moved up to the status date.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsForward;
```

## Examples

Shows how to read/write Prj.MoveCompletedEndsForward property.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsForward, true);

Console.WriteLine("Move Completed Ends Forward: " + project.Get(Prj.MoveCompletedEndsForward));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


