---
title: "Tsk.RemainingOvertimeCost"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La dépense supplémentaire programmée restante pour une tâche"
type: docs
weight: 970
url: /fr/net/aspose.tasks/tsk/remainingovertimecost/
---
## Tsk.RemainingOvertimeCost field

La dépense d’heures supplémentaires prévue restante pour une tâche.

```csharp
public static readonly Key<decimal, TaskKey> RemainingOvertimeCost;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.RemainingOvertimeCost.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeCost, 2m);

Console.WriteLine("Remaining Overtime Cost: " + task.Get(Tsk.RemainingOvertimeCost));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


