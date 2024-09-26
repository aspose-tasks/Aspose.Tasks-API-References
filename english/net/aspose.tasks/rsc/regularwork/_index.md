---
title: Rsc.RegularWork
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The total amount of non overtime work scheduled to be performed by resource
type: docs
weight: 570
url: /net/aspose.tasks/rsc/regularwork/
---
## Rsc.RegularWork field

The total amount of non overtime work scheduled to be performed by resource.

```csharp
public static readonly Key<Duration, RscKey> RegularWork;
```

## Examples

Shows how to read/write Rsc.RegularWork property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + resource.Get(Rsc.RegularWork));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


