---
title: "Prj.TimescaleStart"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. La date à laquelle l’échelle de temps dans la vue commence"
type: docs
weight: 740
url: /fr/net/aspose.tasks/prj/timescalestart/
---
## Prj.TimescaleStart field

La date à laquelle l'échelle de temps dans la vue commence.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleStart;
```

## Exemples

Montre comment définir la date de début de l’échelle de temps pour ajuster la date à laquelle la vue doit commencer.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.TimescaleStart, new DateTime(2012, 4, 30));

Console.WriteLine("Timescale Start: " + project.Get(Prj.TimescaleStart));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


