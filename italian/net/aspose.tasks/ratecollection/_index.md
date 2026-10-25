---
title: "Classe RateCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.RateCollection. Rappresenta una collezione che contiene oggetti Rate."
type: docs
weight: 1630
url: /it/net/aspose.tasks/ratecollection/
---
## RateCollection class

Rappresenta una collezione che contiene oggetti [`Rate`](../rate/).

```csharp
public class RateCollection : IDictionary<RateType, RateByDateCollection>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/ratecollection/count/) { get; } | Restituisce il numero di elementi contenuti nella RateCollection. |
| [IsReadOnly](../../aspose.tasks/ratecollection/isreadonly/) { get; } | Restituisce un valore che indica se questa collezione è di sola lettura. |
| [Item](../../aspose.tasks/ratecollection/item/) { get; set; } | Restituisce o imposta l'elemento all'indice specificato. |
| [ParentResource](../../aspose.tasks/ratecollection/parentresource/) { get; } | Ottiene l'oggetto padre [`Resource`](../resource/) per questa collezione. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/ratecollection/add/#add)(DateTime) | Aggiunge una nuova istanza di [`Rate`](../rate/) a questa collezione. |
| [Add](../../aspose.tasks/ratecollection/add/#add_1)(DateTime, RateType) | Aggiunge una nuova istanza di [`Rate`](../rate/) a questa collezione. |
| [GetEnumerator](../../aspose.tasks/ratecollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Remove](../../aspose.tasks/ratecollection/remove/)(Rate) | Rimuove l'istanza di Rate da questa collezione. |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist)() | Converte l'oggetto `RateCollection` in un elenco di oggetti [`Rate`](../rate/). |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist_1)(RateType) | Converte l'oggetto `RateCollection` in un elenco di oggetti [`Rate`](../rate/) filtrati per il tipo [`RateType`](../ratetype/) specificato. |

## Esempi

Mostra come lavorare con le collezioni di rate.

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

// ottieni l'ultima tariffa mediante accesso per indice
var rateToUpdate = resource.Rates[RateType.B][new DateTime(2019, 11, 12, 8, 0, 0)];
rateToUpdate.RatesTo = new DateTime(2020, 12, 31, 17, 0, 0);
Console.WriteLine("Rates From: " + rateToUpdate.RatesFrom);
Console.WriteLine("Rates To: " + rateToUpdate.RatesTo);

// ...
// lavora con le tariffe
// ...

// rimuovi tutte le tariffe di tipo A
List<Rate> rates = resource.Rates.ToList(RateType.A);
for (var i = 0; i < rates.Count; i++)
{
    var rateToRemove = rates[i];
    resource.Rates.Remove(rateToRemove);
}

// trasforma la collezione di tariffe in un elenco piatto
Console.WriteLine("Iterate over the rates after remove the A-typed values: ");
List<Rate> list = resource.Rates.ToList();
foreach (var rt in list)
{
    Console.WriteLine("Rates From: " + rt.RatesFrom);
    Console.WriteLine("Rates To: " + rt.RatesTo);
    Console.WriteLine("Rate Table: " + rt.RateTable);
}
```

### Vedi anche

* enum [RateType](../ratetype/)
* class [RateByDateCollection](../ratebydatecollection/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


