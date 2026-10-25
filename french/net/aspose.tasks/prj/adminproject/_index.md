---
title: "Prj.AdminProject"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si un projet est un projet administratif"
type: docs
weight: 20
url: /fr/net/aspose.tasks/prj/adminproject/
---
## Prj.AdminProject field

Détermine si un projet est un projet administratif.

```csharp
public static readonly Key<NullableBool, PrjKey> AdminProject;
```

## Exemples

Montre comment lire/écrire la propriété Prj.AdminProject.

```csharp
var project = new Project();

project.Set(Prj.AdminProject, true);

Console.WriteLine("Admin Project: " + project.Get(Prj.AdminProject));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


