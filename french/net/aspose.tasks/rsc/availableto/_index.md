---
title: "Rsc.AvailableTo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. La date de fin à laquelle une ressource est disponible pour travailler aux unités spécifiées pour la période actuelle"
type: docs
weight: 130
url: /fr/net/aspose.tasks/rsc/availableto/
---
## Rsc.AvailableTo field

La date de fin à laquelle une ressource est disponible pour travailler aux unités spécifiées pour la période actuelle.

```csharp
public static readonly Key<DateTime, RscKey> AvailableTo;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.AvailableTo.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableTo, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available To: " + resource.Get(Rsc.AvailableTo));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


