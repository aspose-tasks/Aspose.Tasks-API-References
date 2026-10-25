---
title: "Prj.DateFormat"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Format de date de la vue du projet"
type: docs
weight: 210
url: /fr/net/aspose.tasks/prj/dateformat/
---
## Prj.DateFormat field

Format de date de la vue du projet.

```csharp
public static readonly Key<DateFormat, PrjKey> DateFormat;
```

## Exemples

Montre comment lire/écrire la propriété Prj.DateFormat.

```csharp
var project = new Project();

project.Set(Prj.DateFormat, DateFormat.DateDd);

Console.WriteLine("Date Format: " + project.Get(Prj.DateFormat));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [DateFormat](../../dateformat/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


