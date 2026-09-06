---
title: "Tsk.ActualOvertimeCost"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Coûts engagés pour les heures supplémentaires déjà effectuées sur les tâches par les ressources assignées"
type: docs
weight: 50
url: /fr/net/aspose.tasks/tsk/actualovertimecost/
---
## Tsk.ActualOvertimeCost field

Coûts engagés pour le travail supplémentaire déjà effectué sur les tâches par les ressources assignées.

```csharp
public static readonly Key<decimal, TaskKey> ActualOvertimeCost;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.ActualOvertimeCost.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + task.Get(Tsk.ActualOvertimeCost));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


