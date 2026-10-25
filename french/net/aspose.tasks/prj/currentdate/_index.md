---
title: "Prj.CurrentDate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. La date du système"
type: docs
weight: 190
url: /fr/net/aspose.tasks/prj/currentdate/
---
## Prj.CurrentDate field

La date du système.

```csharp
public static readonly Key<DateTime, PrjKey> CurrentDate;
```

## Exemples

Montre comment lire/écrire la propriété Prj.CurrentDate.

```csharp
var project = new Project();

project.Set(Prj.CurrentDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Current Date: " + project.Get(Prj.CurrentDate));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


