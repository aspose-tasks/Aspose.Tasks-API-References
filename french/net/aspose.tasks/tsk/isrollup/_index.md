---
title: "Tsk.IsRollup"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si les informations sur les barres Gantt des sous‑tâches seront agrégées dans la barre de tâche récapitulative."
type: docs
weight: 690
url: /fr/net/aspose.tasks/tsk/isrollup/
---
## Tsk.IsRollup field

Détermine si les informations sur les barres Gantt des sous‑tâches seront agrégées à la barre de la tâche récapitulative.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRollup;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.IsRollup.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRollup, true);

Console.WriteLine("Is Rollup: " + task.Get(Tsk.IsRollup));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


