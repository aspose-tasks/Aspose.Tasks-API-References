---
title: Rsc.RemainingOvertimeWork
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The amount of remaining scheduled overtime
type: docs
weight: 600
url: /net/aspose.tasks/rsc/remainingovertimework/
---
## Rsc.RemainingOvertimeWork field

The amount of remaining scheduled overtime.

```csharp
public static readonly Key<Duration, RscKey> RemainingOvertimeWork;
```

## Examples

Shows how to read/write Rsc.RemainingOvertimeWork property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + resource.Get(Rsc.RemainingOvertimeWork));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


