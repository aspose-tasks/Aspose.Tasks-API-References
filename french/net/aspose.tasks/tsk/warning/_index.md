---
title: "Tsk.Warning"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Représente le drapeau qui indique que la tâche présente des écarts de planification"
type: docs
weight: 1120
url: /fr/net/aspose.tasks/tsk/warning/
---
## Tsk.Warning field

Représente le drapeau qui indique que la tâche a des écarts de planification.

```csharp
public static readonly Key<bool, TaskKey> Warning;
```

## Exemples

Montre comment lire un avertissement de tâche.

```csharp
var project = new Project(DataDir + "schedule-conflict.mpp");
var task = project.RootTask.Children.GetById(1);
Console.WriteLine(task.Get(Tsk.Warning));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


