---
title: "Tsk.DisplayOnTimeline"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Spécifie si une tâche doit être affichée dans une vue chronologique"
type: docs
weight: 290
url: /fr/net/aspose.tasks/tsk/displayontimeline/
---
## Tsk.DisplayOnTimeline field

Spécifie si une tâche doit être affichée dans la vue chronologique.

```csharp
public static readonly Key<bool, TaskKey> DisplayOnTimeline;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.DisplayOnTimeline.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayOnTimeline, true);

Console.WriteLine("Display On Timeline: " + task.Get(Tsk.DisplayOnTimeline));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


