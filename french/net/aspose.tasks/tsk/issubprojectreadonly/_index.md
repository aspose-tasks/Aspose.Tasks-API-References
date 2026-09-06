---
title: "Tsk.IsSubprojectReadOnly"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si un sous‑projet est en lecture seule"
type: docs
weight: 710
url: /fr/net/aspose.tasks/tsk/issubprojectreadonly/
---
## Tsk.IsSubprojectReadOnly field

Détermine si un sous‑projet est en lecture seule.

```csharp
public static readonly Key<NullableBool, TaskKey> IsSubprojectReadOnly;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.IsSubprojectReadOnly.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubprojectReadOnly, true);

Console.WriteLine("Is Subproject Read Only: " + task.Get(Tsk.IsSubprojectReadOnly));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


