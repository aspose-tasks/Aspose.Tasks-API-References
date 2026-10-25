---
title: "Rsc.ActualWorkProtected"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le montant de travail à travers lequel le travail réel est protégé"
type: docs
weight: 80
url: /fr/net/aspose.tasks/rsc/actualworkprotected/
---
## Rsc.ActualWorkProtected field

Le montant de travail à travers lequel le travail réel est protégé.

```csharp
public static readonly Key<Duration, RscKey> ActualWorkProtected;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.ActualWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + resource.Get(Rsc.ActualWorkProtected));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


