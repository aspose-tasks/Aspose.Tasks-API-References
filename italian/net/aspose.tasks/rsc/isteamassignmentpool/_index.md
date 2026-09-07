---
title: "Rsc.IsTeamAssignmentPool"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Mostra se la risorsa corrente è una risorsa di squadra"
type: docs
weight: 430
url: /it/net/aspose.tasks/rsc/isteamassignmentpool/
---
## Rsc.IsTeamAssignmentPool field

Mostra se la risorsa corrente è una risorsa di team.

```csharp
public static readonly Key<bool, RscKey> IsTeamAssignmentPool;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.IsTeamAssignmentPool.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsTeamAssignmentPool, true);

Console.WriteLine("Is Team Assignment Pool: " + resource.Get(Rsc.IsTeamAssignmentPool));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


