---
title: "Rsc.Work"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le temps total prévu pour une ressource sur une tâche"
type: docs
weight: 690
url: /fr/net/aspose.tasks/rsc/work/
---
## Rsc.Work field

Le montant total de temps prévu pour une ressource sur une tâche.

```csharp
public static readonly Key<Duration, RscKey> Work;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.Work.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Work, project.GetWork(1));

Console.WriteLine("Work: " + resource.Get(Rsc.Work));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


