---
title: "Prj.AutoAddNewResourcesAndTasks"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si de nouvelles ressources ou tâches sont automatiquement ajoutées à un pool de ressources ou de tâches"
type: docs
weight: 50
url: /fr/net/aspose.tasks/prj/autoaddnewresourcesandtasks/
---
## Prj.AutoAddNewResourcesAndTasks field

Détermine si de nouvelles ressources ou tâches sont automatiquement ajoutées à un pool de ressources ou de tâches.

```csharp
public static readonly Key<NullableBool, PrjKey> AutoAddNewResourcesAndTasks;
```

## Exemples

Montre comment lire/écrire la propriété Prj.AutoAddNewResourcesAndTasks.

```csharp
var project = new Project();

project.Set(Prj.AutoAddNewResourcesAndTasks, true);

Console.WriteLine("Auto Add New Resources And Tasks: " + project.Get(Prj.AutoAddNewResourcesAndTasks));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


