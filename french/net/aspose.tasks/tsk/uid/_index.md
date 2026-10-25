---
title: "Tsk.Uid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. L'Id unique d'une tâche."
type: docs
weight: 1110
url: /fr/net/aspose.tasks/tsk/uid/
---
## Tsk.Uid field

L'identifiant unique d'une tâche.

```csharp
public static readonly Key<int, TaskKey> Uid;
```

## Exemples

Montre comment lire/écrire les propriétés des tâches.

```csharp
var project = new Project();

// Ajouter une tâche et définir les propriétés de la tâche
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analyser toutes les tâches collectées
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


