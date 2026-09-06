---
title: "Prj.DurationFormat"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Le format pour exprimer la durée totale"
type: docs
weight: 300
url: /fr/net/aspose.tasks/prj/durationformat/
---
## Prj.DurationFormat field

Le format d'expression de la durée globale.

```csharp
public static readonly Key<TimeUnitType, PrjKey> DurationFormat;
```

## Exemples

Montre comment lire/écrire la propriété Prj.DurationFormat.

```csharp
var project = new Project();

project.Set(Prj.DurationFormat, TimeUnitType.Day);

Console.WriteLine("Duration Format: " + project.Get(Prj.DurationFormat));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


