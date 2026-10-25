---
title: "Tsk.LateStart"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La dernière date à laquelle une tâche peut commencer sans retarder la fin du projet"
type: docs
weight: 740
url: /fr/net/aspose.tasks/tsk/latestart/
---
## Tsk.LateStart field

La date la plus tardive à laquelle une tâche peut commencer sans retarder la fin du projet.

```csharp
public static readonly Key<DateTime, TaskKey> LateStart;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.LateStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Start: " + task.Get(Tsk.LateStart));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


