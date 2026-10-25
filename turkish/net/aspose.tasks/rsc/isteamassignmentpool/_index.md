---
title: "Rsc.IsTeamAssignmentPool"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Mevcut kaynağın bir takım kaynağı olup olmadığını gösterir"
type: docs
weight: 430
url: /tr/net/aspose.tasks/rsc/isteamassignmentpool/
---
## Rsc.IsTeamAssignmentPool field

Mevcut kaynağın bir ekip kaynağı olup olmadığını gösterir.

```csharp
public static readonly Key<bool, RscKey> IsTeamAssignmentPool;
```

## Örnekler

Rsc.IsTeamAssignmentPool özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsTeamAssignmentPool, true);

Console.WriteLine("Is Team Assignment Pool: " + resource.Get(Rsc.IsTeamAssignmentPool));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


