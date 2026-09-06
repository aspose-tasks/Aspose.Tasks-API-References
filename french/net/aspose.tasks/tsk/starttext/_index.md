---
title: "Tsk.StartText"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Tsk field. Retourne le texte de début de la tâche"
type: docs
weight: 1030
url: /fr/net/aspose.tasks/tsk/starttext/
---
## Tsk.StartText field

Renvoie le texte de début de la tâche.

```csharp
public static readonly Key<string, TaskKey> StartText;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.StartText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartText, "Start Task Text");

Console.WriteLine("Start Text: " + task.Get(Tsk.StartText));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


