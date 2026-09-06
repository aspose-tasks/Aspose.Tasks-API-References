---
title: "Tsk.ActualStart"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La date et l'heure auxquelles une tâche a réellement commencé"
type: docs
weight: 80
url: /fr/net/aspose.tasks/tsk/actualstart/
---
## Tsk.ActualStart field

La date et l'heure auxquelles une tâche a réellement commencé.

```csharp
public static readonly Key<DateTime, TaskKey> ActualStart;
```

## Exemples

Montre que les dates du projet sont réinitialisées en mode d'évaluation.

```csharp
var project = new Project();

// créer de nouvelles tâches
var task1 = project.RootTask.Children.Add("Task1");
task1.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task1.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

var task2 = project.RootTask.Children.Add("Task2");
task2.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task2.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

project.Save(OutDir + "EvaluationDateTimeLimitations_out.xml", SaveFileFormat.Xml);
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


