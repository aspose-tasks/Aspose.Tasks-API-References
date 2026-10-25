---
title: "Tsk.HideBar"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Tsk field. Détermine si la barre Gantt d'une tâche est masquée lorsqu'elle est affichée dans Microsoft Project"
type: docs
weight: 480
url: /fr/net/aspose.tasks/tsk/hidebar/
---
## Tsk.HideBar field

Détermine si la barre Gantt d’une tâche est masquée lorsqu’elle est affichée dans Microsoft Project.

```csharp
public static readonly Key<NullableBool, TaskKey> HideBar;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.HideBar.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.HideBar, true);

Console.WriteLine("Hide Bar: " + task.Get(Tsk.HideBar));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


