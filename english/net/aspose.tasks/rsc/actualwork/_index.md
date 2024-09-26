---
title: Rsc.ActualWork
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The amount of work that has already been done by resource assigned to tasks
type: docs
weight: 70
url: /net/aspose.tasks/rsc/actualwork/
---
## Rsc.ActualWork field

The amount of work that has already been done by resource assigned to tasks.

```csharp
public static readonly Key<Duration, RscKey> ActualWork;
```

## Examples

Shows how to read/write Rsc.ActualWork property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + resource.Get(Rsc.ActualWork));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


