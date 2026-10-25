---
title: "Tsk.Duration"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. L’ensemble total du temps de travail actif d’une tâche tel qu’il est saisi ou calculé par Microsoft Project en fonction de la date de début, de la date de fin, des calendriers et d’autres facteurs de planification."
type: docs
weight: 300
url: /fr/net/aspose.tasks/tsk/duration/
---
## Tsk.Duration field

La durée totale du temps de travail actif pour une tâche telle qu'elle a été saisie ou calculée par Microsoft Project en fonction de la date de début, de la date de fin, des calendriers et d'autres facteurs de planification.

```csharp
public static readonly Key<Duration, TaskKey> Duration;
```

## Exemples

Montre comment définir la durée de la tâche.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddTaskDuration_out.xml", SaveFileFormat.Xml);
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


