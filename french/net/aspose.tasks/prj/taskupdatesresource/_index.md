---
title: "Prj.TaskUpdatesResource"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si les mises à jour des tâches mettent à jour les ressources"
type: docs
weight: 710
url: /fr/net/aspose.tasks/prj/taskupdatesresource/
---
## Prj.TaskUpdatesResource field

Détermine si les mises à jour des tâches mettent à jour les ressources.

```csharp
public static readonly Key<NullableBool, PrjKey> TaskUpdatesResource;
```

## Exemples

Montre comment lire/écrire la propriété Prj.TaskUpdatesResource.

```csharp
var project = new Project();

project.Set(Prj.TaskUpdatesResource, true);

Console.WriteLine("Task Updates Resource: " + project.Get(Prj.TaskUpdatesResource));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


