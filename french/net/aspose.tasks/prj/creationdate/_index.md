---
title: "Prj.CreationDate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. La date et l'heure de création d'un projet"
type: docs
weight: 130
url: /fr/net/aspose.tasks/prj/creationdate/
---
## Prj.CreationDate field

La date et l'heure de création d'un projet.

```csharp
public static readonly Key<DateTime, PrjKey> CreationDate;
```

## Remarques

Enregistré au format UTC dans les fichiers mpp. Type DateTime.

## Exemples

Montre comment lire/écrire la propriété Prj.CreationDate.

```csharp
var project = new Project();

project.Set(Prj.CreationDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Creation Date: " + project.Get(Prj.CreationDate));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


