---
title: Rsc.Work
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The total amount of time scheduled for a resource on a task
type: docs
weight: 690
url: /net/aspose.tasks/rsc/work/
---
## Rsc.Work field

The total amount of time scheduled for a resource on a task.

```csharp
public static readonly Key<Duration, RscKey> Work;
```

## Examples

Shows how to read/write Rsc.Work property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Work, project.GetWork(1));

Console.WriteLine("Work: " + resource.Get(Rsc.Work));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


