---
title: "Rsc.IsTeamAssignmentPool"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Indique si la ressource actuelle est une ressource d'équipe"
type: docs
weight: 430
url: /fr/net/aspose.tasks/rsc/isteamassignmentpool/
---
## Rsc.IsTeamAssignmentPool field

Indique si la ressource actuelle est une ressource d'équipe.

```csharp
public static readonly Key<bool, RscKey> IsTeamAssignmentPool;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.IsTeamAssignmentPool.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsTeamAssignmentPool, true);

Console.WriteLine("Is Team Assignment Pool: " + resource.Get(Rsc.IsTeamAssignmentPool));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


