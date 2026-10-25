---
title: "Rsc.ActualWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. La quantité de travail déjà effectuée par la ressource affectée aux tâches"
type: docs
weight: 70
url: /fr/net/aspose.tasks/rsc/actualwork/
---
## Rsc.ActualWork field

Le montant de travail qui a déjà été effectué par la ressource affectée aux tâches.

```csharp
public static readonly Key<Duration, RscKey> ActualWork;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.ActualWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + resource.Get(Rsc.ActualWork));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


