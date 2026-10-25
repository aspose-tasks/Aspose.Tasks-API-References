---
title: "Rsc.RegularWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le montant total du travail non supplémentaire prévu pour être effectué par la ressource"
type: docs
weight: 570
url: /fr/net/aspose.tasks/rsc/regularwork/
---
## Rsc.RegularWork field

Le montant total du travail non supplémentaire prévu à être effectué par la ressource.

```csharp
public static readonly Key<Duration, RscKey> RegularWork;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.RegularWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + resource.Get(Rsc.RegularWork));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


