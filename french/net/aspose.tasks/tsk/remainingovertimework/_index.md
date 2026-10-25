---
title: "Tsk.RemainingOvertimeWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le montant du temps supplémentaire programmé restant."
type: docs
weight: 980
url: /fr/net/aspose.tasks/tsk/remainingovertimework/
---
## Tsk.RemainingOvertimeWork field

Le montant du temps d’heures supplémentaires prévu restant.

```csharp
public static readonly Key<Duration, TaskKey> RemainingOvertimeWork;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.RemainingOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + task.Get(Tsk.RemainingOvertimeWork));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


