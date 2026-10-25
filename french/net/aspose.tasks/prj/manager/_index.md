---
title: "Prj.Manager"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Le responsable d'un projet"
type: docs
weight: 450
url: /fr/net/aspose.tasks/prj/manager/
---
## Prj.Manager field

Le responsable du projet.

```csharp
public static readonly Key<string, PrjKey> Manager;
```

## Exemples

Montre comment lire/écrire la propriété Prj.Manager.

```csharp
var project = new Project();

project.Set(Prj.Manager, "Steve");

Console.WriteLine("Manager: " + project.Get(Prj.Manager));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


