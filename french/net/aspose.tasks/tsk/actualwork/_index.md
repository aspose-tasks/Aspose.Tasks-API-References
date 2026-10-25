---
title: "Tsk.ActualWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La quantité de travail déjà effectuée par les ressources assignées aux tâches"
type: docs
weight: 90
url: /fr/net/aspose.tasks/tsk/actualwork/
---
## Tsk.ActualWork field

Le montant de travail déjà effectué par les ressources affectées aux tâches.

```csharp
public static readonly Key<Duration, TaskKey> ActualWork;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.ActualWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + task.Get(Tsk.ActualWork));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


