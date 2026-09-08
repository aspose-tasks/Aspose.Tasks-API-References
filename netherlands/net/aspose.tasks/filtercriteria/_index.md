---
title: "Class FilterCriteria"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.FilterCriteria class. Definieert de criteria waaraan taken of resources moeten voldoen om weergegeven te worden in de MSP-weergave"
type: docs
weight: 630
url: /nl/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

Definieert de criteria waaraan taken of resources moeten voldoen om weergegeven te worden in de MSP-weergave.

```csharp
public class FilterCriteria
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | De standaardconstructor. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | Haalt de lijst op van onderliggende `FilterCriteria`-rijen. Als het filter meer dan één criteriumrij bevat, is het effect van een EN-operator dat de criteria voor beide rijen moeten worden voldaan zodat de taak of resource wordt weergegeven als resultaat van dit filter. Het effect van een OF-operator is dat de criteria voor de ene of de andere rij moeten worden voldaan. |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | Haalt op of stelt een [`Field`](./field/) in om te wijzigen. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | Haalt op of stelt het criterium in dat is vastgesteld met FieldName, Test en Value en dat betrekking heeft op andere criteria in het filter. |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | Haalt op of stelt het type vergelijking in dat wordt gemaakt tussen FieldName en Value en dat dient als selectiecriterium voor het filter. [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | Haalt de objectwaarden op om te vergelijken met de waarde van het veld dat is gespecificeerd met FieldName. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [IsFieldValue](../../aspose.tasks/filtercriteria/isfieldvalue/)() | Haalt op of de rechterwaarde van FilterCriteria een veldreferentie is, geen constante waarde. |
| [SetValueField](../../aspose.tasks/filtercriteria/setvaluefield/)(Field) | Stelt het veld in waarvan de waarde wordt vergeleken met de waarde van het veld dat is gespecificeerd door FieldName. |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | Retourneert de tekenreeksrepresentatie van de instantie van de `FilterCriteria`-klasse. |

## Voorbeelden

Toont hoe taakfiltercriteria te lezen.

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine("Count of criteria rows: " + filter.Criteria.CriteriaRows.Count);
foreach (var row in filter.Criteria.CriteriaRows)
{
    Console.WriteLine("Field: " + row.Field);
    Console.WriteLine("Operation: " + row.Operation);
    Console.WriteLine("Test: " + row.Test);

    var values = row.Values.Where(c => c != null).ToArray();
    if (values.Length == 0)
    {
        continue;
    }

    Console.WriteLine("Value{0}: {1}", values.Length == 1 ? "" : "s", string.Join(", ", values));
}

// printfiltercriteria als een tekenreeks 
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine("Criteria filter 1:");
Console.WriteLine(criteria1.ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);
Console.WriteLine("Criteria filter 2:");
Console.WriteLine(criteria2.ToString());

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine("Criteria filter 21:");
Console.WriteLine(criteria21.ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine("Criteria filter 22:");
Console.WriteLine(criteria22.ToString());
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


