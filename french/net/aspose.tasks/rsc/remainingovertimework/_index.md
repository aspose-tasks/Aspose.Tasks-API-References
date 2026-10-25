---
title: "Rsc.RemainingOvertimeWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le montant du temps supplémentaire programmé restant"
type: docs
weight: 600
url: /fr/net/aspose.tasks/rsc/remainingovertimework/
---
## Rsc.RemainingOvertimeWork field

Le montant du temps supplémentaire prévu restant.

```csharp
public static readonly Key<Duration, RscKey> RemainingOvertimeWork;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.RemainingOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + resource.Get(Rsc.RemainingOvertimeWork));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


