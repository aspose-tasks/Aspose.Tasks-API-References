---
title: "Rsc.AvailableFrom"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. La date de début à laquelle une ressource est disponible pour travailler aux unités spécifiées pour la période actuelle"
type: docs
weight: 120
url: /fr/net/aspose.tasks/rsc/availablefrom/
---
## Rsc.AvailableFrom field

La date de début à laquelle une ressource est disponible pour travailler aux unités spécifiées pour la période actuelle.

```csharp
public static readonly Key<DateTime, RscKey> AvailableFrom;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.AvailableFrom.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableFrom, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available From: " + resource.Get(Rsc.AvailableFrom));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


