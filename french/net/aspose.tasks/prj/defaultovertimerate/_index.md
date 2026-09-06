---
title: "Prj.DefaultOvertimeRate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Le taux d'heures supplémentaires par défaut pour les nouvelles ressources"
type: docs
weight: 250
url: /fr/net/aspose.tasks/prj/defaultovertimerate/
---
## Prj.DefaultOvertimeRate field

Le taux d'heures supplémentaires par défaut pour les nouvelles ressources.

```csharp
public static readonly Key<double, PrjKey> DefaultOvertimeRate;
```

## Exemples

Montre comment lire les propriétés par défaut du projet.

```csharp
var project = new Project(DataDir + "DefaultProperties.mpp");

// Définir les propriétés par défaut
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, DateTime.Now);
project.Set(Prj.DefaultStartTime, project.Get(Prj.StartDate));
project.Set(Prj.DefaultTaskType, TaskType.FixedDuration);
project.Set(Prj.DefaultStandardRate, 15);
project.Set(Prj.DefaultOvertimeRate, 12);
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
project.Set(Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated);

// Afficher les propriétés par défaut
Console.WriteLine("New Task Default Start: " + project.Get(Prj.DefaultStartTime).ToShortDateString());
Console.WriteLine("New Task Default Type: " + project.Get(Prj.DefaultTaskType));
Console.WriteLine("Resource Default Standard Rate: " + project.Get(Prj.DefaultStandardRate));
Console.WriteLine("Resource Default Overtime Rate: " + project.Get(Prj.DefaultOvertimeRate));
Console.WriteLine("Default Task EV Method: " + project.Get(Prj.DefaultTaskEVMethod));
Console.WriteLine("Default Cost Accrual: " + project.Get(Prj.DefaultFixedCostAccrual));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


