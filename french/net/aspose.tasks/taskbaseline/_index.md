---
title: "Classe TaskBaseline"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.TaskBaseline. Représente la ligne de base d'une tâche"
type: docs
weight: 2370
url: /fr/net/aspose.tasks/taskbaseline/
---
## TaskBaseline class

Représente la ligne de base d'une tâche.

```csharp
public sealed class TaskBaseline : Baseline, IComparable<TaskBaseline>, IEquatable<TaskBaseline>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TaskBaseline](taskbaseline/)(Task) | Initialise une nouvelle instance de la classe `TaskBaseline`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Obtient ou définit le numéro unique d'un enregistrement de données de ligne de base. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Obtient ou définit le coût budgété d'un travail effectué par une ressource pour un projet à ce jour. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Obtient ou définit le coût budgété d'un travail planifié pour une ressource. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Obtient ou définit le coût projeté d'une ressource lorsque la ligne de base est enregistrée. |
| [Duration](../../aspose.tasks/taskbaseline/duration/) { get; set; } | Obtient ou définit la durée prévue de la tâche lorsque la ligne de base a été enregistrée. |
| [EstimatedDuration](../../aspose.tasks/taskbaseline/estimatedduration/) { get; set; } | Obtient ou définit une valeur indiquant si la durée de la ligne de base de la tâche était estimée. |
| [Finish](../../aspose.tasks/taskbaseline/finish/) { get; set; } | Obtient ou définit la date de fin prévue de la tâche lorsque la ligne de base a été enregistrée. |
| [FixedCost](../../aspose.tasks/taskbaseline/fixedcost/) { get; set; } | Obtient ou définit un coût fixe de la tâche lorsque la ligne de base a été enregistrée. |
| [Interim](../../aspose.tasks/taskbaseline/interim/) { get; set; } | Obtient ou définit une valeur indiquant s’il s’agit d’une ligne de base intermédiaire. |
| [Start](../../aspose.tasks/taskbaseline/start/) { get; set; } | Obtient ou définit la date de début prévue de la tâche lorsque la ligne de base a été enregistrée. |
| [TimephasedData](../../aspose.tasks/taskbaseline/timephaseddata/) { get; set; } | Obtient ou définit une instance de `TimephasedDataCollection` pour cet objet. Les données temporelles associées à la ligne de base de la tâche. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Obtient ou définit le travail assigné à une ressource lorsque la ligne de base est enregistrée. Le montant de travail assigné à une ressource lorsque la ligne de base a été enregistrée. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | Implémentation de l'interface IComparable. Compare cette instance à l'objet Baseline spécifié. |
| [CompareTo](../../aspose.tasks/taskbaseline/compareto/#compareto_1)(TaskBaseline) | Implémentation de l'interface IComparable. Compare cette instance à l'objet Baseline spécifié. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| override [Equals](../../aspose.tasks/taskbaseline/equals/#equals_2)(object) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [Equals](../../aspose.tasks/taskbaseline/equals/#equals_1)(TaskBaseline) | Renvoie une valeur indiquant si cette instance est égale à l’objet `TaskBaseline` spécifié. |
| override [GetHashCode](../../aspose.tasks/taskbaseline/gethashcode/)() | Renvoie une valeur de code de hachage pour l’instance de la classe `TaskBaseline`. |

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

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


