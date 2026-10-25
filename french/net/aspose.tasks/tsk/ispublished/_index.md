---
title: "Tsk.IsPublished"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si la tâche actuelle doit être publiée sur Project Server avec le reste du projet"
type: docs
weight: 660
url: /fr/net/aspose.tasks/tsk/ispublished/
---
## Tsk.IsPublished field

Détermine si la tâche actuelle doit être publiée sur Project Server avec le reste du projet.

```csharp
public static readonly Key<NullableBool, TaskKey> IsPublished;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.IsPublished.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsPublished, true);

Console.WriteLine("Is Published: " + task.Get(Tsk.IsPublished));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


