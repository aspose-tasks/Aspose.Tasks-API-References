---
title: "Rsc.Start"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. La date à laquelle une ressource assignée est prévue de commencer à travailler sur une tâche"
type: docs
weight: 640
url: /fr/net/aspose.tasks/rsc/start/
---
## Rsc.Start field

La date à laquelle une ressource assignée est prévue pour commencer à travailler sur une tâche.

```csharp
public static readonly Key<DateTime, RscKey> Start;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.Start.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Start, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Start: " + resource.Get(Rsc.Start));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


