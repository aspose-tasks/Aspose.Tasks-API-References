---
title: "Tsk.ManualStart"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Définit le démarrage programmé manuellement d'une tâche"
type: docs
weight: 800
url: /fr/net/aspose.tasks/tsk/manualstart/
---
## Tsk.ManualStart field

Définit la date de début planifiée manuellement d’une tâche.

```csharp
public static readonly Key<DateTime, TaskKey> ManualStart;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.ManualStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Start: " + task.Get(Tsk.ManualStart));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


