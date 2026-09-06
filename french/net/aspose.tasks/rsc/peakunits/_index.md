---
title: "Rsc.PeakUnits"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. L'unité d'affectation maximale pour une ressource à un moment donné pour toutes les tâches auxquelles la ressource est affectée"
type: docs
weight: 540
url: /fr/net/aspose.tasks/rsc/peakunits/
---
## Rsc.PeakUnits field

L'unité d'affectation maximale pour une ressource à un moment donné pour toutes les tâches auxquelles la ressource est assignée.

```csharp
public static readonly Key<double, RscKey> PeakUnits;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.PeakUnits.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.PeakUnits, 2);

Console.WriteLine("Peak Units: " + resource.Get(Rsc.PeakUnits));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


