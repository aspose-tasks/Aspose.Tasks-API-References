---
title: Prj.MoveCompletedEndsBack
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether the end of completed portions of tasks scheduled to start after the status date but started earlier should be moved back to the status date
type: docs
weight: 490
url: /net/aspose.tasks/prj/movecompletedendsback/
---
## Prj.MoveCompletedEndsBack field

Determines whether the end of completed portions of tasks scheduled to start after the status date but started earlier should be moved back to the status date.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsBack;
```

## Examples

Shows how to read/write Prj.MoveCompletedEndsBack property.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsBack, true);

Console.WriteLine("Move Completed Ends Back: " + project.Get(Prj.MoveCompletedEndsBack));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


