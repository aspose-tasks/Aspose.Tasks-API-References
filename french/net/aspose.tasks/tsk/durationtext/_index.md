---
title: "Tsk.DurationText"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Retourne le texte de durée de la tâche"
type: docs
weight: 310
url: /fr/net/aspose.tasks/tsk/durationtext/
---
## Tsk.DurationText field

Renvoie le texte de la durée de la tâche.

```csharp
public static readonly Key<string, TaskKey> DurationText;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.DurationText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationText, "Not A Duration");

Console.WriteLine("Duration Text: " + task.Get(Tsk.DurationText));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


