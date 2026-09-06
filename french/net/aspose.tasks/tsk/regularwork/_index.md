---
title: "Tsk.RegularWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le montant total de travail hors heures supplémentaires prévu pour être effectué par les ressources"
type: docs
weight: 940
url: /fr/net/aspose.tasks/tsk/regularwork/
---
## Tsk.RegularWork field

Le montant total du travail non supplémentaire prévu pour être effectué par les ressources.

```csharp
public static readonly Key<Duration, TaskKey> RegularWork;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.RegularWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + task.Get(Tsk.RegularWork));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


