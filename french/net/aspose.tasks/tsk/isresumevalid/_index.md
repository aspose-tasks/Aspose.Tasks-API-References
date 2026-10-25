---
title: "Tsk.IsResumeValid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si une tâche peut être reprise"
type: docs
weight: 680
url: /fr/net/aspose.tasks/tsk/isresumevalid/
---
## Tsk.IsResumeValid field

Détermine si une tâche peut être reprise.

```csharp
public static readonly Key<NullableBool, TaskKey> IsResumeValid;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.IsResumeValid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsResumeValid, true);

Console.WriteLine("Is Resume Valid: " + task.Get(Tsk.IsResumeValid));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


