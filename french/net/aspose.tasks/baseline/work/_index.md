---
title: "Baseline.Work"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Baseline. Obtient ou définit le travail attribué à une ressource lorsque la ligne de base est enregistrée. Le montant du travail attribué à une ressource lorsque la ligne de base a été enregistrée"
type: docs
weight: 60
url: /fr/net/aspose.tasks/baseline/work/
---
## Baseline.Work property

Obtient ou définit le travail assigné à une ressource lorsque la ligne de base est enregistrée. Le montant de travail assigné à une ressource lorsque la ligne de base a été enregistrée.

```csharp
public Duration Work { get; set; }
```

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

* struct [Duration](../../duration/)
* class [Baseline](../)
* namespace [Aspose.Tasks](../../baseline/)
* assembly [Aspose.Tasks](../../../)


