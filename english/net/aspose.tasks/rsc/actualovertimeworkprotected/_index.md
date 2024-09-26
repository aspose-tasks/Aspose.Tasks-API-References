---
title: Rsc.ActualOvertimeWorkProtected
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The amount of work through which actual overtime work is protected
type: docs
weight: 60
url: /net/aspose.tasks/rsc/actualovertimeworkprotected/
---
## Rsc.ActualOvertimeWorkProtected field

The amount of work through which actual overtime work is protected.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWorkProtected;
```

## Examples

Shows how to read/write Rsc.ActualOvertimeWorkProtected property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + resource.Get(Rsc.ActualOvertimeWorkProtected));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


