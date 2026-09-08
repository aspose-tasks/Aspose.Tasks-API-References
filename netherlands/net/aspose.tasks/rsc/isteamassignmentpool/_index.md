---
title: "Rsc.IsTeamAssignmentPool"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. Toont of de huidige resource een teamresource is"
type: docs
weight: 430
url: /nl/net/aspose.tasks/rsc/isteamassignmentpool/
---
## Rsc.IsTeamAssignmentPool field

Toont of de huidige resource een teamresource is.

```csharp
public static readonly Key<bool, RscKey> IsTeamAssignmentPool;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.IsTeamAssignmentPool te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsTeamAssignmentPool, true);

Console.WriteLine("Is Team Assignment Pool: " + resource.Get(Rsc.IsTeamAssignmentPool));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


