---
title: "Tsk.EarlyStart"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La date la plus tôt à laquelle une tâche peut commencer, basée sur les dates de début anticipé des tâches prédécesseurs et successeurs ainsi que d'autres contraintes."
type: docs
weight: 340
url: /fr/net/aspose.tasks/tsk/earlystart/
---
## Tsk.EarlyStart field

La date la plus tôt à laquelle une tâche pourrait éventuellement commencer, basée sur les dates de début anticipées des tâches prédécesseurs et successeurs et d'autres contraintes.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyStart;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.EarlyStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Start: " + task.Get(Tsk.EarlyStart));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


