---
title: "Tsk.Guid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Les codes d’identification uniques générés pour une tâche"
type: docs
weight: 460
url: /fr/net/aspose.tasks/tsk/guid/
---
## Tsk.Guid field

Les codes d'identification uniques générés pour une tâche.

```csharp
public static readonly Key<string, TaskKey> Guid;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.Guid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Guid, "60648d59-9c2b-4dc6-bfdb-bfd38f331d61");

Console.WriteLine("Guid: " + task.Get(Tsk.Guid));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


