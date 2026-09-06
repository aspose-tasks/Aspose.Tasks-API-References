---
title: "Rsc.ActualOvertimeWorkProtected"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le montant de travail à travers lequel le travail supplémentaire réel est protégé"
type: docs
weight: 60
url: /fr/net/aspose.tasks/rsc/actualovertimeworkprotected/
---
## Rsc.ActualOvertimeWorkProtected field

Le montant de travail à travers lequel le travail supplémentaire réel est protégé.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWorkProtected;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.ActualOvertimeWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + resource.Get(Rsc.ActualOvertimeWorkProtected));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


