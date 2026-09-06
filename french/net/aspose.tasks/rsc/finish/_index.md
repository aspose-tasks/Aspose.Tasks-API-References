---
title: "Rsc.Finish"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. La date à laquelle une ressource doit terminer le travail sur toutes les tâches assignées"
type: docs
weight: 290
url: /fr/net/aspose.tasks/rsc/finish/
---
## Rsc.Finish field

La date à laquelle une ressource est prévue pour terminer le travail sur toutes les tâches affectées.

```csharp
public static readonly Key<DateTime, RscKey> Finish;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.Finish.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Finish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Finish: " + resource.Get(Rsc.Finish));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


