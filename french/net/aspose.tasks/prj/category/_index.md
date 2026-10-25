---
title: "Prj.Category"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. La catégorie d'un projet"
type: docs
weight: 100
url: /fr/net/aspose.tasks/prj/category/
---
## Prj.Category field

La catégorie d'un projet.

```csharp
public static readonly Key<string, PrjKey> Category;
```

## Exemples

Montre comment lire/écrire la propriété Prj.Category.

```csharp
var project = new Project();

project.Set(Prj.Category, "Special");

Console.WriteLine("Category: " + project.Get(Prj.Category));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


