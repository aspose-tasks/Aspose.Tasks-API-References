---
title: "Klasse AssignmentBaseline"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.AssignmentBaseline klasse. Vertegenwoordigt de baseline van een resource‑toewijzing"
type: docs
weight: 50
url: /nl/net/aspose.tasks/assignmentbaseline/
---
## AssignmentBaseline class

Stelt de basislijn van een resource‑toewijzing voor.

```csharp
public class AssignmentBaseline : Baseline, IComparable<AssignmentBaseline>, 
    IEquatable<AssignmentBaseline>
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [AssignmentBaseline](assignmentbaseline/)() | De standaardconstructor. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Haalt op of stelt het unieke nummer van een baseline-gegevensrecord in. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Haalt op of stelt de begrote kosten van een door een resource uitgevoerd werk voor een project tot nu toe in. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Haalt op of stelt de budgetkosten van een voor een resource gepland werk in. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Haalt op of stelt de geprojecteerde kosten van een resource in wanneer de baseline wordt opgeslagen. |
| [Finish](../../aspose.tasks/assignmentbaseline/finish/) { get; set; } | Haalt op of stelt de geplande einddatum van de resource‑toewijzing in wanneer de baseline werd opgeslagen. De einddatum van de resource‑toewijzing wanneer deze baseline werd opgeslagen. |
| [Start](../../aspose.tasks/assignmentbaseline/start/) { get; set; } | Haalt op of stelt de geplande startdatum van de resource‑toewijzing in wanneer de baseline werd opgeslagen. De startdatum van de resource‑toewijzing wanneer deze baseline werd opgeslagen. |
| [TimephasedData](../../aspose.tasks/assignmentbaseline/timephaseddata/) { get; set; } | Haalt op of stelt de [`TimephasedDataCollection`](../timephaseddatacollection/)‑instantie voor dit object in. De tijdgephaseerde gegevens die zijn gekoppeld aan de resource‑toewijzingsbaseline. Retourneert de [`TimephasedDataCollection`](../timephaseddatacollection/)‑instantie voor dit object. De collectie van tijdgephaseerde gegevens die aan deze baseline zijn gekoppeld. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Haalt op of stelt het werk in dat aan een resource is toegewezen wanneer de baseline wordt opgeslagen. De hoeveelheid toegewezen werk aan een resource wanneer de baseline werd opgeslagen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [CompareTo](../../aspose.tasks/assignmentbaseline/compareto/#compareto)(AssignmentBaseline) | IComparable‑interface‑implementatie. Vergelijkt deze instantie met het opgegeven Baseline‑object. |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | IComparable‑interface‑implementatie. Vergelijkt deze instantie met het opgegeven Baseline‑object. |
| [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals)(AssignmentBaseline) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven AssignmentBaseline-object. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| override [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals_2)(object) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| override [GetHashCode](../../aspose.tasks/assignmentbaseline/gethashcode/)() |  |

## Voorbeelden

Toont hoe te werken met baselines van toewijzingen.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// toewijzingsbaselines worden ingesteld wanneer men de baseline voor het hele project instelt
project.SetBaseline(BaselineType.Baseline);

// lees toewijzingsbaseline‑informatie
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

// controleer baseline‑gelijkheid
var assn1 = project.ResourceAssignments.GetByUid(5);
var assn2 = project.ResourceAssignments.GetByUid(7);

var assignmentBaseline1 = assn1.Baselines.ToList()[0];
var assignmentBaseline2 = assn2.Baselines.ToList()[0];

// baselines kunnen worden vergeleken door gebruik te maken van 'Equals'-methodoverloads
Console.WriteLine("Are baselines equal: " + assignmentBaseline1.Equals(assignmentBaseline2));

// of door gebruik te maken van overladen rekenkundige bewerkingen
Console.WriteLine("Is baseline 1 less than baseline 2: " + (assignmentBaseline1 < assignmentBaseline2));

// de hashcode van de baseline is gebaseerd op het baselinenummer
Console.WriteLine("Assignment baseline 1 hashcode: " + assignmentBaseline1.GetHashCode());
Console.WriteLine("Assignment baseline 2 hashcode: " + assignmentBaseline2.GetHashCode());
```

### Zie ook

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


