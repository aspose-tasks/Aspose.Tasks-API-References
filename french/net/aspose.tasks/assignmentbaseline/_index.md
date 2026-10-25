---
title: "Classe AssignmentBaseline"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.AssignmentBaseline. Représente la ligne de base d'une affectation de ressource"
type: docs
weight: 50
url: /fr/net/aspose.tasks/assignmentbaseline/
---
## AssignmentBaseline class

Représente la ligne de base d'une affectation de ressource.

```csharp
public class AssignmentBaseline : Baseline, IComparable<AssignmentBaseline>, 
    IEquatable<AssignmentBaseline>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [AssignmentBaseline](assignmentbaseline/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Obtient ou définit le numéro unique d'un enregistrement de données de ligne de base. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Obtient ou définit le coût budgété d'un travail effectué par une ressource pour un projet à ce jour. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Obtient ou définit le coût budgété d'un travail planifié pour une ressource. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Obtient ou définit le coût projeté d'une ressource lorsque la ligne de base est enregistrée. |
| [Finish](../../aspose.tasks/assignmentbaseline/finish/) { get; set; } | Obtient ou définit la date de fin prévue de l'affectation de la ressource lorsque la ligne de base a été enregistrée. La date de fin de l'affectation de la ressource lorsque cette ligne de base a été enregistrée. |
| [Start](../../aspose.tasks/assignmentbaseline/start/) { get; set; } | Obtient ou définit la date de début prévue de l'affectation de la ressource lorsque la ligne de base a été enregistrée. La date de début de l'affectation de la ressource lorsque cette ligne de base a été enregistrée. |
| [TimephasedData](../../aspose.tasks/assignmentbaseline/timephaseddata/) { get; set; } | Obtient ou définit l'instance [`TimephasedDataCollection`](../timephaseddatacollection/) pour cet objet. Les données temporelles associées à la ligne de base de l'affectation de la ressource. renvoie l'instance [`TimephasedDataCollection`](../timephaseddatacollection/) pour cet objet. La collection de données temporelles associées à cette ligne de base. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Obtient ou définit le travail assigné à une ressource lorsque la ligne de base est enregistrée. Le montant de travail assigné à une ressource lorsque la ligne de base a été enregistrée. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CompareTo](../../aspose.tasks/assignmentbaseline/compareto/#compareto)(AssignmentBaseline) | Implémentation de l'interface IComparable. Compare cette instance à l'objet Baseline spécifié. |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | Implémentation de l'interface IComparable. Compare cette instance à l'objet Baseline spécifié. |
| [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals)(AssignmentBaseline) | Renvoie une valeur indiquant si cette instance est égale à l'objet AssignmentBaseline spécifié. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| override [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals_2)(object) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| override [GetHashCode](../../aspose.tasks/assignmentbaseline/gethashcode/)() |  |

## Exemples

Montre comment travailler avec les lignes de base des affectations.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// Les lignes de base d'affectation sont définies lorsqu'on définit la ligne de base sur l'ensemble du projet
project.SetBaseline(BaselineType.Baseline);

// Lire les informations de ligne de base d'affectation
foreach (var assignment in project.ResourceAssignments)
{
    foreach (var baseline in assignment.Baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
        Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
        if (baseline.TimephasedData != null)
        {
            foreach (var td in baseline.TimephasedData)
            {
                Console.WriteLine("TD Start: " + td.Start);
                Console.WriteLine("TD Finish: " + td.Finish);
                Console.WriteLine("TD Timephased Data Type: " + td.TimephasedDataType);
                Console.WriteLine();
            }
        }

        Console.WriteLine();
    }

    Console.WriteLine();
}

// Vérifier l'égalité des lignes de base
var assn1 = project.ResourceAssignments.GetByUid(5);
var assn2 = project.ResourceAssignments.GetByUid(7);

var assignmentBaseline1 = assn1.Baselines.ToList()[0];
var assignmentBaseline2 = assn2.Baselines.ToList()[0];

// Les lignes de base peuvent être comparées en utilisant les surcharges de la méthode 'Equals'
Console.WriteLine("Are baselines equal: " + assignmentBaseline1.Equals(assignmentBaseline2));

// ou en utilisant une opération arithmétique surchargée
Console.WriteLine("Is baseline 1 less than baseline 2: " + (assignmentBaseline1 < assignmentBaseline2));

// Le code de hachage de la ligne de base est basé sur le numéro de la ligne de base
Console.WriteLine("Assignment baseline 1 hashcode: " + assignmentBaseline1.GetHashCode());
Console.WriteLine("Assignment baseline 2 hashcode: " + assignmentBaseline2.GetHashCode());
```

### Voir aussi

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


