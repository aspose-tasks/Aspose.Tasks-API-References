---
title: "Tsk.IgnoreWarnings"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Indique s'il faut masquer l'indicateur d'avertissement de conflit d'horaire dans Microsoft Project"
type: docs
weight: 540
url: /fr/net/aspose.tasks/tsk/ignorewarnings/
---
## Tsk.IgnoreWarnings field

Indique s’il faut masquer l’indicateur d’avertissement de conflit d’horaire dans Microsoft Project.

```csharp
public static readonly Key<bool, TaskKey> IgnoreWarnings;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.IgnoreWarnings.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreWarnings, true);

Console.WriteLine("Ignore Warnings: " + task.Get(Tsk.IgnoreWarnings));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


