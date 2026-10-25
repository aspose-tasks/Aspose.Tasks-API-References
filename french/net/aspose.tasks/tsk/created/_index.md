---
title: "Tsk.Created"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Tsk field. La date à laquelle une tâche a été créée"
type: docs
weight: 250
url: /fr/net/aspose.tasks/tsk/created/
---
## Tsk.Created field

La date à laquelle une tâche a été créée.

```csharp
public static readonly Key<DateTime, TaskKey> Created;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.Created.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + task.Get(Tsk.Created));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


