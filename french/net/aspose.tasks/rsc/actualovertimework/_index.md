---
title: "Rsc.ActualOvertimeWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le montant réel de travail supplémentaire déjà effectué par la ressource assignée aux tâches"
type: docs
weight: 50
url: /fr/net/aspose.tasks/rsc/actualovertimework/
---
## Rsc.ActualOvertimeWork field

Le montant réel du travail supplémentaire déjà effectué par la ressource affectée aux tâches.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWork;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.ActualOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + resource.Get(Rsc.ActualOvertimeWork));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


