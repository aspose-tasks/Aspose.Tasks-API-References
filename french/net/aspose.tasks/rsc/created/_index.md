---
title: "Rsc.Created"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. La date et l’heure auxquelles une ressource a été ajoutée au projet"
type: docs
weight: 260
url: /fr/net/aspose.tasks/rsc/created/
---
## Rsc.Created field

La date et l'heure auxquelles une ressource a été ajoutée au projet.

```csharp
public static readonly Key<DateTime, RscKey> Created;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.Created.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + resource.Get(Rsc.Created));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


