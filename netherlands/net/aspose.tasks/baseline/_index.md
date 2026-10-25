---
title: "Klasse Baseline"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Baseline klasse. Vertegenwoordigt baseline-waarden van een resource"
type: docs
weight: 110
url: /nl/net/aspose.tasks/baseline/
---
## Baseline class

Geeft de baseline-waarden van een resource weer.

```csharp
public class Baseline : IComparable<Baseline>, IEquatable<Baseline>
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [Baseline](baseline/)() | De standaardconstructor. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Haalt op of stelt het unieke nummer van een baseline-gegevensrecord in. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Haalt op of stelt de begrote kosten van een door een resource uitgevoerd werk voor een project tot nu toe in. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Haalt op of stelt de budgetkosten van een voor een resource gepland werk in. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Haalt op of stelt de geprojecteerde kosten van een resource in wanneer de baseline wordt opgeslagen. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Haalt op of stelt het werk in dat aan een resource is toegewezen wanneer de baseline wordt opgeslagen. De hoeveelheid toegewezen werk aan een resource wanneer de baseline werd opgeslagen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | IComparable‑interface‑implementatie. Vergelijkt deze instantie met het opgegeven Baseline‑object. |
| [Equals](../../aspose.tasks/baseline/equals/#equals)(Baseline) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| override [Equals](../../aspose.tasks/baseline/equals/#equals_1)(object) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| override [GetHashCode](../../aspose.tasks/baseline/gethashcode/)() | Retourneert een hashcode-waarde voor de baseline. |
| [operator ==](../../aspose.tasks/baseline/op_equality/) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [operator &gt;](../../aspose.tasks/baseline/op_greaterthan/) | Retourneert een waarde die aangeeft of deze instantie groter is dan een opgegeven object. |
| [operator &gt;=](../../aspose.tasks/baseline/op_greaterthanorequal/) | Retourneert een waarde die aangeeft of deze instantie groter dan of gelijk aan een opgegeven object is. |
| [operator !=](../../aspose.tasks/baseline/op_inequality/) | Retourneert een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object. |
| [operator &lt;](../../aspose.tasks/baseline/op_lessthan/) | Retourneert een waarde die aangeeft of deze instantie kleiner is dan een opgegeven object. |
| [operator &lt;=](../../aspose.tasks/baseline/op_lessthanorequal/) | Retourneert een waarde die aangeeft of deze instantie kleiner dan of gelijk aan een opgegeven object is. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


