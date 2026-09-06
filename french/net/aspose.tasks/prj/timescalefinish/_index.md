---
title: "Prj.TimescaleFinish"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. La date à laquelle l’échelle de temps dans la vue se termine"
type: docs
weight: 730
url: /fr/net/aspose.tasks/prj/timescalefinish/
---
## Prj.TimescaleFinish field

La date à laquelle l'échelle de temps dans la vue se termine.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleFinish;
```

## Exemples

Montre comment lire/écrire la propriété Prj.TimescaleFinish.

```csharp
var project = new Project();

project.Set(Prj.TimescaleFinish, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Timescale Finish: " + project.Get(Prj.TimescaleFinish));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


