---
title: Rsc.ActualWorkProtected
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The amount of work through which actual work is protected
type: docs
weight: 80
url: /net/aspose.tasks/rsc/actualworkprotected/
---
## Rsc.ActualWorkProtected field

The amount of work through which actual work is protected.

```csharp
public static readonly Key<Duration, RscKey> ActualWorkProtected;
```

## Examples

Shows how to read/write Rsc.ActualWorkProtected property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + resource.Get(Rsc.ActualWorkProtected));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


