---
title: Rsc.ActualOvertimeWork
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The actual amount of overtime work already performed by resource assigned to tasks
type: docs
weight: 50
url: /net/aspose.tasks/rsc/actualovertimework/
---
## Rsc.ActualOvertimeWork field

The actual amount of overtime work already performed by resource assigned to tasks.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWork;
```

## Examples

Shows how to read/write Rsc.ActualOvertimeWork property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + resource.Get(Rsc.ActualOvertimeWork));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


