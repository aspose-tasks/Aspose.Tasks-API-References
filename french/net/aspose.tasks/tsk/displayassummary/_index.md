---
title: "Tsk.DisplayAsSummary"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si la tâche doit être affichée comme tâche de synthèse. Lecture prise en charge uniquement pour le format XML"
type: docs
weight: 280
url: /fr/net/aspose.tasks/tsk/displayassummary/
---
## Tsk.DisplayAsSummary field

Détermine si la tâche doit être affichée comme une tâche récapitulative. Lecture prise en charge uniquement pour le format XML.

```csharp
public static readonly Key<NullableBool, TaskKey> DisplayAsSummary;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.DisplayAsSummary.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayAsSummary, true);

Console.WriteLine("Display As Summary: " + task.Get(Tsk.DisplayAsSummary));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


