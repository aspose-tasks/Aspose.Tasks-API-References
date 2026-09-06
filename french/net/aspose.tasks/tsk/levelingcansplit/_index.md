---
title: "Tsk.LevelingCanSplit"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si la fonction d'équilibrage des ressources peut provoquer des découpages du travail restant sur cette tâche"
type: docs
weight: 760
url: /fr/net/aspose.tasks/tsk/levelingcansplit/
---
## Tsk.LevelingCanSplit field

Détermine si la fonction de nivellement des ressources peut provoquer des divisions du travail restant sur cette tâche.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelingCanSplit;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.LevelingCanSplit.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingCanSplit, true);

Console.WriteLine("Leveling Can Split: " + task.Get(Tsk.LevelingCanSplit));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


