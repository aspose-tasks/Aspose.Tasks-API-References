---
title: "Rsc.MaterialLabel"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. L'unité de mesure pour la ressource matérielle"
type: docs
weight: 440
url: /fr/net/aspose.tasks/rsc/materiallabel/
---
## Rsc.MaterialLabel field

L'unité de mesure pour la ressource matérielle.

```csharp
public static readonly Key<string, RscKey> MaterialLabel;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.MaterialLabel.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaterialLabel, "kg");

Console.WriteLine("Material Label: " + resource.Get(Rsc.MaterialLabel));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


