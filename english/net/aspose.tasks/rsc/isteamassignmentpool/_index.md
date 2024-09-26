---
title: Rsc.IsTeamAssignmentPool
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. Shows whether the current resource is a team resource
type: docs
weight: 430
url: /net/aspose.tasks/rsc/isteamassignmentpool/
---
## Rsc.IsTeamAssignmentPool field

Shows whether the current resource is a team resource.

```csharp
public static readonly Key<bool, RscKey> IsTeamAssignmentPool;
```

## Examples

Shows how to read/write Rsc.IsTeamAssignmentPool property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsTeamAssignmentPool, true);

Console.WriteLine("Is Team Assignment Pool: " + resource.Get(Rsc.IsTeamAssignmentPool));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


