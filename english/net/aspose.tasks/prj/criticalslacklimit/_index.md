---
title: Prj.CriticalSlackLimit
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The number of days to the end of a task when Microsoft Project marks that task as a critical task
type: docs
weight: 140
url: /net/aspose.tasks/prj/criticalslacklimit/
---
## Prj.CriticalSlackLimit field

The number of days to the end of a task when Microsoft Project marks that task as a critical task.

```csharp
public static readonly Key<int, PrjKey> CriticalSlackLimit;
```

## Examples

Shows how to read/write Prj.CriticalSlackLimit property.

```csharp
var project = new Project();

project.Set(Prj.CriticalSlackLimit, 2);

Console.WriteLine("Critical Slack Limit: " + project.Get(Prj.CriticalSlackLimit));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


