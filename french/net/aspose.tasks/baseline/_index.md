---
title: "Classe Baseline"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Baseline. Représente les valeurs de base d'une ressource"
type: docs
weight: 110
url: /fr/net/aspose.tasks/baseline/
---
## Baseline class

Représente les valeurs de base d'une ressource.

```csharp
public class Baseline : IComparable<Baseline>, IEquatable<Baseline>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Baseline](baseline/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Obtient ou définit le numéro unique d'un enregistrement de données de ligne de base. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Obtient ou définit le coût budgété d'un travail effectué par une ressource pour un projet à ce jour. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Obtient ou définit le coût budgété d'un travail planifié pour une ressource. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Obtient ou définit le coût projeté d'une ressource lorsque la ligne de base est enregistrée. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Obtient ou définit le travail assigné à une ressource lorsque la ligne de base est enregistrée. Le montant de travail assigné à une ressource lorsque la ligne de base a été enregistrée. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | Implémentation de l'interface IComparable. Compare cette instance à l'objet Baseline spécifié. |
| [Equals](../../aspose.tasks/baseline/equals/#equals)(Baseline) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| override [Equals](../../aspose.tasks/baseline/equals/#equals_1)(object) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| override [GetHashCode](../../aspose.tasks/baseline/gethashcode/)() | Renvoie une valeur de code de hachage pour la baseline. |
| [operator ==](../../aspose.tasks/baseline/op_equality/) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [operator &gt;](../../aspose.tasks/baseline/op_greaterthan/) | Renvoie une valeur indiquant si cette instance est supérieure à un objet spécifié. |
| [operator &gt;=](../../aspose.tasks/baseline/op_greaterthanorequal/) | Renvoie une valeur indiquant si cette instance est supérieure ou égale à un objet spécifié. |
| [operator !=](../../aspose.tasks/baseline/op_inequality/) | Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié. |
| [operator &lt;](../../aspose.tasks/baseline/op_lessthan/) | Renvoie une valeur indiquant si cette instance est inférieure à un objet spécifié. |
| [operator &lt;=](../../aspose.tasks/baseline/op_lessthanorequal/) | Renvoie une valeur indiquant si cette instance est inférieure ou égale à un objet spécifié. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


