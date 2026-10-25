---
title: "Tsk.FinishText"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Retourne le texte de fin de la tâche"
type: docs
weight: 410
url: /fr/net/aspose.tasks/tsk/finishtext/
---
## Tsk.FinishText field

Renvoie le texte de fin de la tâche.

```csharp
public static readonly Key<string, TaskKey> FinishText;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.FinishText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishText, "Not A Finish");

Console.WriteLine("Finish Text: " + task.Get(Tsk.FinishText));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


