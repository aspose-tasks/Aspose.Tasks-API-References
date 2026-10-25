---
title: "Prj.CustomDateFormat"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Format de date personnalisé de la vue du projet. Utilisé pour formater les dates lorsque la propriété DateFormat est définie sur Custom"
type: docs
weight: 200
url: /fr/net/aspose.tasks/prj/customdateformat/
---
## Prj.CustomDateFormat field

Format de date personnalisé de la vue du projet. Utilisé pour formater les dates lorsque la propriété [`DateFormat`](../dateformat/) est définie sur Custom.

```csharp
public static readonly Key<string, PrjKey> CustomDateFormat;
```

## Exemples

Montre comment lire/écrire la propriété Prj.CustomDateFormat.

```csharp
var project = new Project();

project.Set(Prj.CustomDateFormat, "dd MMMM yyyy H:mm");

Console.WriteLine("Custom Date Format: " + project.Get(Prj.CustomDateFormat));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


