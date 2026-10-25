---
title: "Prj.StatusDate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. La date d'état pour afficher la progression ou calculer les totaux de la valeur acquise. La date d'état est la même que la date actuelle, sauf si une date d'état différente est spécifiée"
type: docs
weight: 690
url: /fr/net/aspose.tasks/prj/statusdate/
---
## Prj.StatusDate field

la date d'état pour afficher la progression ou calculer les totaux de la valeur acquise. La date d'état est la même que la date actuelle (date d'aujourd'hui) sauf si une autre date d'état est spécifiée.

```csharp
public static readonly Key<DateTime, PrjKey> StatusDate;
```

## Exemples

Montre comment lire/écrire la propriété Prj.StatusDate.

```csharp
var project = new Project();

project.Set(Prj.StatusDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Status Date: " + project.Get(Prj.StatusDate));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


