---
title: "Tsk.PhysicalPercentComplete"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Valeur de pourcentage d'achèvement qui peut être utilisée comme alternative pour calculer le coût budgété du travail effectué (BCWP)"
type: docs
weight: 900
url: /fr/net/aspose.tasks/tsk/physicalpercentcomplete/
---
## Tsk.PhysicalPercentComplete field

Valeur de pourcentage d’achèvement qui peut être utilisée comme alternative pour calculer le coût budgété du travail effectué (BCWP).

```csharp
public static readonly Key<int, TaskKey> PhysicalPercentComplete;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.PhysicalPercentComplete.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PhysicalPercentComplete, 10);

Console.WriteLine("Physical Percent Complete: " + task.Get(Tsk.PhysicalPercentComplete));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


