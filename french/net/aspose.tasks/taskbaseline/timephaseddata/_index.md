---
title: "TaskBaseline.TimephasedData"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété TaskBaseline. Obtient ou définit une instance de TimephasedDataCollection pour cet objet. Les données temporelles associées à la ligne de base de la tâche"
type: docs
weight: 80
url: /fr/net/aspose.tasks/taskbaseline/timephaseddata/
---
## TaskBaseline.TimephasedData property

Obtient ou définit une instance de `TimephasedDataCollection` pour cet objet. Les données temporelles associées à la ligne de base de la tâche.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
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

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


