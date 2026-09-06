---
title: "Tsk.ActualOvertimeWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le montant réel de travail supplémentaire déjà effectué par les ressources affectées aux tâches."
type: docs
weight: 60
url: /fr/net/aspose.tasks/tsk/actualovertimework/
---
## Tsk.ActualOvertimeWork field

Le montant réel du travail supplémentaire déjà effectué par les ressources affectées aux tâches.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWork;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.ActualOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + task.Get(Tsk.ActualOvertimeWork));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


