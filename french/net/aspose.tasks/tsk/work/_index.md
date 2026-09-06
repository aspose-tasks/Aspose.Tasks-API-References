---
title: "Tsk.Work"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le temps total prévu sur une tâche pour toutes les ressources assignées"
type: docs
weight: 1150
url: /fr/net/aspose.tasks/tsk/work/
---
## Tsk.Work field

Le temps total planifié sur une tâche pour toutes les ressources affectées.

```csharp
public static readonly Key<Duration, TaskKey> Work;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.Work.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Work, project.GetWork(1));

Console.WriteLine("Work: " + task.Get(Tsk.Work));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


