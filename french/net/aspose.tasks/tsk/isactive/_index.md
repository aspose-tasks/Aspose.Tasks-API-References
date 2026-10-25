---
title: "Tsk.IsActive"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si une tâche est active. Les tâches inactives n'affectent plus les autres tâches ni le calendrier global du projet."
type: docs
weight: 550
url: /fr/net/aspose.tasks/tsk/isactive/
---
## Tsk.IsActive field

Détermine si une tâche est active. Les tâches inactives n’affectent plus les autres tâches ni le planning global du projet.

```csharp
public static readonly Key<NullableBool, TaskKey> IsActive;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.IsActive.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsActive, true);

Console.WriteLine("Is Active: " + task.Get(Tsk.IsActive));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


