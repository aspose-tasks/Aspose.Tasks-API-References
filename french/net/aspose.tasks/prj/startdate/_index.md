---
title: "Prj.StartDate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. La date de début d'un projet"
type: docs
weight: 680
url: /fr/net/aspose.tasks/prj/startdate/
---
## Prj.StartDate field

La date de début d'un projet.

```csharp
public static readonly Key<DateTime, PrjKey> StartDate;
```

## Exemples

Montre comment lire/écrire la propriété Prj.StartDate.

```csharp
var project = new Project();

project.Set(Prj.StartDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Start Date: " + project.Get(Prj.StartDate));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


