---
title: "RateCollection.Remove"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος RateCollection. Αφαιρεί το αντικείμενο Rate από αυτή τη συλλογή"
type: docs
weight: 70
url: /el/net/aspose.tasks/ratecollection/remove/
---
## RateCollection.Remove method

Αφαιρεί το στιγμιότυπο Rate από αυτή τη συλλογή.

```csharp
public bool Remove(Rate item)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | Rate | Το στοιχείο προς αφαίρεση. |

### Τιμή Επιστροφής

true εάν το συγκεκριμένο Rate αφαιρέθηκε επιτυχώς· διαφορετικά, false.

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές τιμών.

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

// λάβετε την πιο πρόσφατη τιμή μέσω πρόσβασης δείκτη
var rateToUpdate = resource.Rates[RateType.B][new DateTime(2019, 11, 12, 8, 0, 0)];
rateToUpdate.RatesTo = new DateTime(2020, 12, 31, 17, 0, 0);
Console.WriteLine("Rates From: " + rateToUpdate.RatesFrom);
Console.WriteLine("Rates To: " + rateToUpdate.RatesTo);

// ...
// εργαστείτε με τιμές
// ...

// αφαιρέστε όλες τις τιμές τύπου A
List<Rate> rates = resource.Rates.ToList(RateType.A);
for (var i = 0; i < rates.Count; i++)
{
    var rateToRemove = rates[i];
    resource.Rates.Remove(rateToRemove);
}

// μετατρέψτε τη συλλογή τιμών σε μια επίπεδη λίστα
Console.WriteLine("Iterate over the rates after remove the A-typed values: ");
List<Rate> list = resource.Rates.ToList();
foreach (var rt in list)
{
    Console.WriteLine("Rates From: " + rt.RatesFrom);
    Console.WriteLine("Rates To: " + rt.RatesTo);
    Console.WriteLine("Rate Table: " + rt.RateTable);
}
```

### Δείτε επίσης

* class [Rate](../../rate/)
* class [RateCollection](../)
* namespace [Aspose.Tasks](../../ratecollection/)
* assembly [Aspose.Tasks](../../../)


