---
title: "Prj.Name"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Le nom du projet"
type: docs
weight: 540
url: /fr/net/aspose.tasks/prj/name/
---
## Prj.Name field

Le nom du projet.

```csharp
public static readonly Key<string, PrjKey> Name;
```

## Exemples

Montre comment lire/écrire le nom du projet.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

project.Set(Prj.Name, "Custom Project Name");

Console.WriteLine("Project name: " + project.Get(Prj.Name));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


