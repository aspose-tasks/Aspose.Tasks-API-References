---
title: "Rsc.Phonetics"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. L’orthographe phonétique du nom de la ressource. À n’utiliser qu’avec le japonais."
type: docs
weight: 560
url: /fr/net/aspose.tasks/rsc/phonetics/
---
## Rsc.Phonetics field

L'orthographe phonétique du nom de la ressource. À utiliser uniquement avec le japonais.

```csharp
public static readonly Key<string, RscKey> Phonetics;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.Phonetics.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Phonetics, "Phonetics");

Console.WriteLine("Phonetics: " + resource.Get(Rsc.Phonetics));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


