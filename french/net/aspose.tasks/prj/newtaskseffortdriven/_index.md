---
title: "Prj.NewTasksEffortDriven"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si les nouvelles tâches sont basées sur l'effort"
type: docs
weight: 560
url: /fr/net/aspose.tasks/prj/newtaskseffortdriven/
---
## Prj.NewTasksEffortDriven field

Détermine si les nouvelles tâches sont à effort.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksEffortDriven;
```

## Exemples

Montre comment lire/écrire la propriété Prj.NewTasksEffortDriven.

```csharp
var project = new Project();

project.Set(Prj.NewTasksEffortDriven, true);

Console.WriteLine("New Tasks Effort Driven: " + project.Get(Prj.NewTasksEffortDriven));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


