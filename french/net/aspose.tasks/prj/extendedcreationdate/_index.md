---
title: "Prj.ExtendedCreationDate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Date utilisée pour le calcul et le reporting"
type: docs
weight: 320
url: /fr/net/aspose.tasks/prj/extendedcreationdate/
---
## Prj.ExtendedCreationDate field

Date utilisée pour le calcul et le reporting.

```csharp
public static readonly Key<DateTime, PrjKey> ExtendedCreationDate;
```

## Exemples

Montre comment lire/écrire la propriété Prj.ExtendedCreationDate.

```csharp
var project = new Project();

project.Set(Prj.ExtendedCreationDate, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Extended Creation Date: " + project.Get(Prj.ExtendedCreationDate));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


