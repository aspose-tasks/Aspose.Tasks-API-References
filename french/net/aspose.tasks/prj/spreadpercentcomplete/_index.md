---
title: "Prj.SpreadPercentComplete"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si un pourcentage d'achèvement est réparti à la date d'état"
type: docs
weight: 670
url: /fr/net/aspose.tasks/prj/spreadpercentcomplete/
---
## Prj.SpreadPercentComplete field

Détermine si le pourcentage d'avancement est réparti jusqu'à la date d'état.

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadPercentComplete;
```

## Exemples

Montre comment lire/écrire la propriété Prj.SpreadPercentComplete.

```csharp
var project = new Project();

project.Set(Prj.SpreadPercentComplete, true);

Console.WriteLine("Spread Percent Complete: " + project.Get(Prj.SpreadPercentComplete));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


