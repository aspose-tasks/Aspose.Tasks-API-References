---
title: "Rsc.RemainingWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le temps encore nécessaire pour terminer une tâche ou un ensemble de tâches"
type: docs
weight: 610
url: /fr/net/aspose.tasks/rsc/remainingwork/
---
## Rsc.RemainingWork field

Le temps encore nécessaire pour terminer une tâche ou un ensemble de tâches.

```csharp
public static readonly Key<Duration, RscKey> RemainingWork;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.RemainingWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + resource.Get(Rsc.RemainingWork));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


