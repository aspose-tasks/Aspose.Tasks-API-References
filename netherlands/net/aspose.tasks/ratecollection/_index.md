---
title: "Class RateCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.RateCollection class. Stelt een collectie voor die Rate‑objecten bevat."
type: docs
weight: 1630
url: /nl/net/aspose.tasks/ratecollection/
---
## RateCollection class

Stelt een collectie voor die [`Rate`](../rate/) objecten bevat.

```csharp
public class RateCollection : IDictionary<RateType, RateByDateCollection>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/ratecollection/count/) { get; } | Geeft het aantal elementen terug dat in de RateCollection zit. |
| [IsReadOnly](../../aspose.tasks/ratecollection/isreadonly/) { get; } | Geeft een waarde terug die aangeeft of deze collectie alleen‑lezen is. |
| [Item](../../aspose.tasks/ratecollection/item/) { get; set; } | Retourneert of stelt het element in op de opgegeven index. |
| [ParentResource](../../aspose.tasks/ratecollection/parentresource/) { get; } | Haalt het bovenliggende [`Resource`](../resource/) object op voor deze collectie. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/ratecollection/add/#add)(DateTime) | Voegt een nieuw [`Rate`](../rate/) exemplaar toe aan deze collectie. |
| [Add](../../aspose.tasks/ratecollection/add/#add_1)(DateTime, RateType) | Voegt een nieuw [`Rate`](../rate/) exemplaar toe aan deze collectie. |
| [GetEnumerator](../../aspose.tasks/ratecollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks/ratecollection/remove/)(Rate) | Verwijdert Rate instance uit deze collectie. |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist)() | Converteert het `RateCollection`‑object naar een lijst van [`Rate`](../rate/) objecten. |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist_1)(RateType) | Converteert het `RateCollection`‑object naar een lijst van [`Rate`](../rate/) objecten gefilterd op het opgegeven [`RateType`](../ratetype/) type. |

## Voorbeelden

Toont hoe te werken met rate‑collecties.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Test Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0), RateType.B);
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;

Console.WriteLine("Print rates of '{0}' resource: ", resource.Rates.ParentResource.Get(Rsc.Name));
Console.WriteLine("Count of rates: {0}", resource.Rates.Count);
Console.WriteLine("Is rate collection read-only: {0}", resource.Rates.IsReadOnly);
foreach (KeyValuePair<RateType, RateByDateCollection> sortedRates in resource.Rates)
{
    foreach (KeyValuePair<DateTime, Rate> pair in sortedRates.Value)
    {
        var rate = pair.Value;
        Console.WriteLine("Rates From: " + rate.RatesFrom);
        Console.WriteLine("Rates To: " + rate.RatesTo);
        Console.WriteLine("Rate Table: " + rate.RateTable);
        Console.WriteLine();
    }
}

// haal de nieuwste rate op via indextoegang
var rateToUpdate = resource.Rates[RateType.B][new DateTime(2019, 11, 12, 8, 0, 0)];
rateToUpdate.RatesTo = new DateTime(2020, 12, 31, 17, 0, 0);
Console.WriteLine("Rates From: " + rateToUpdate.RatesFrom);
Console.WriteLine("Rates To: " + rateToUpdate.RatesTo);

// ...
// werken met rates
// ...

// verwijder alle rates van type A
List<Rate> rates = resource.Rates.ToList(RateType.A);
for (var i = 0; i < rates.Count; i++)
{
    var rateToRemove = rates[i];
    resource.Rates.Remove(rateToRemove);
}

// transformeer de rate‑collectie naar een platte lijst
Console.WriteLine("Iterate over the rates after remove the A-typed values: ");
List<Rate> list = resource.Rates.ToList();
foreach (var rt in list)
{
    Console.WriteLine("Rates From: " + rt.RatesFrom);
    Console.WriteLine("Rates To: " + rt.RatesTo);
    Console.WriteLine("Rate Table: " + rt.RateTable);
}
```

### Zie ook

* enum [RateType](../ratetype/)
* class [RateByDateCollection](../ratebydatecollection/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


