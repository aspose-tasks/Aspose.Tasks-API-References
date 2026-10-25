---
title: "Prj.LastPrinted"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Dernière impression du projet. Enregistrée au format UTC dans les fichiers mpp. Type DateTime"
type: docs
weight: 430
url: /fr/net/aspose.tasks/prj/lastprinted/
---
## Prj.LastPrinted field

Dernière impression du projet. Enregistrée au format UTC dans les fichiers mpp. Type DateTime.

```csharp
public static readonly Key<DateTime, PrjKey> LastPrinted;
```

## Exemples

Montre comment lire/écrire la propriété Prj.LastPrinted.

```csharp
var project = new Project();

project.Set(Prj.LastPrinted, new DateTime(2020, 4, 10, 13, 0, 0));

Console.WriteLine("Last Printed: " + project.Get(Prj.LastPrinted));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


