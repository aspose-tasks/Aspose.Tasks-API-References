---
title: Rsc.RemainingWork
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The time still required to complete a task or set of tasks
type: docs
weight: 610
url: /net/aspose.tasks/rsc/remainingwork/
---
## Rsc.RemainingWork field

The time still required to complete a task or set of tasks.

```csharp
public static readonly Key<Duration, RscKey> RemainingWork;
```

## Examples

Shows how to read/write Rsc.RemainingWork property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + resource.Get(Rsc.RemainingWork));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


