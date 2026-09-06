---
title: "Tsk.IsMarked"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Indique si une tâche est marquée pour une action supplémentaire ou une identification d'un certain type"
type: docs
weight: 620
url: /fr/net/aspose.tasks/tsk/ismarked/
---
## Tsk.IsMarked field

Indique si une tâche est marquée pour une action supplémentaire ou une identification quelconque.

```csharp
public static readonly Key<bool, TaskKey> IsMarked;
```

## Remarques

S'applique uniquement au format de fichier mpp.

## Exemples

Montre comment lire/écrire la propriété Tsk.IsMarked.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsMarked, true);

Console.WriteLine("Is Marked: " + task.Get(Tsk.IsMarked));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


