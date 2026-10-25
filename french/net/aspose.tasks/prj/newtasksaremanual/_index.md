---
title: "Prj.NewTasksAreManual"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si les nouvelles tâches sont créées en mode manuel"
type: docs
weight: 550
url: /fr/net/aspose.tasks/prj/newtasksaremanual/
---
## Prj.NewTasksAreManual field

Détermine si les nouvelles tâches sont créées comme manuelles.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksAreManual;
```

## Exemples

Montre comment lire/écrire la propriété Prj.NewTasksAreManual.

```csharp
var project = new Project();

project.Set(Prj.NewTasksAreManual, true);

Console.WriteLine("New Tasks Are Manual: " + project.Get(Prj.NewTasksAreManual));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


