---
title: "Baseline.CompareTo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Baseline method. Implémentation de l'interface IComparable. Compare cette instance à l'objet Baseline spécifié"
type: docs
weight: 70
url: /fr/net/aspose.tasks/baseline/compareto/
---
## Baseline.CompareTo method

Implémentation de l'interface IComparable. Compare cette instance à l'objet Baseline spécifié.

```csharp
public int CompareTo(Baseline other)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| autre | Baseline | l'objet Baseline spécifié avec lequel comparer cette instance. |

### Valeur de retour

renvoie -1 si cette instance est inférieure à l'objet spécifié, 1 si cette instance est supérieure à l'objet spécifié ; sinon renvoie 0

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

* class [Baseline](../)
* namespace [Aspose.Tasks](../../baseline/)
* assembly [Aspose.Tasks](../../../)


