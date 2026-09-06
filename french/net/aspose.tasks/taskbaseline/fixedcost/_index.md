---
title: "TaskBaseline.FixedCost"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété TaskBaseline. Obtient ou définit un coût fixe de la tâche lorsque la ligne de base a été enregistrée"
type: docs
weight: 50
url: /fr/net/aspose.tasks/taskbaseline/fixedcost/
---
## TaskBaseline.FixedCost property

Obtient ou définit un coût fixe de la tâche lorsque la ligne de base a été enregistrée.

```csharp
public double FixedCost { get; set; }
```

## Exemples

Montre comment accéder à une information de ligne de base.

```csharp
var project = new Project();

// Création de TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Afficher la durée de la ligne de base de la tâche
var baseline = task.Baselines.ToList()[0];
Console.WriteLine("Baseline Start: {0}", baseline.Start);
Console.WriteLine("Baseline duration: {0}", baseline.Duration);
Console.WriteLine("Baseline duration format: {0}", baseline.Duration.TimeUnit);
Console.WriteLine("Is it estimated duration?: {0}", baseline.EstimatedDuration);
Console.WriteLine("Baseline Finish: {0}", baseline.Finish);

// valeur indiquant s’il s’agit d’une ligne de base intermédiaire
Console.WriteLine("Interim: {0}", baseline.Interim);
Console.WriteLine("Fixed Cost: {0}", baseline.FixedCost);

// imprimer les données temporelles de la ligne de base de la tâche
Console.WriteLine("Number of timephased items: " + baseline.TimephasedData.Count);
foreach (var data in baseline.TimephasedData)
{
    Console.WriteLine(" Uid: " + data.Uid);
    Console.WriteLine(" Start: " + data.Start);
    Console.WriteLine(" Finish: " + data.Finish);
}
```

### Voir aussi

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


