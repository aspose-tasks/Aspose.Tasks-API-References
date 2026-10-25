---
title: "Classe AvailabilityPeriodCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.AvailabilityPeriodCollection. Rappresenta una collezione che contiene oggetti AvailabilityPeriod"
type: docs
weight: 90
url: /it/net/aspose.tasks/availabilityperiodcollection/
---
## AvailabilityPeriodCollection class

Rappresenta una collezione che contiene oggetti [`AvailabilityPeriod`](../availabilityperiod/).

```csharp
public class AvailabilityPeriodCollection : IList<AvailabilityPeriod>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/availabilityperiodcollection/count/) { get; } | Ottiene il numero di elementi contenuti in questa collezione. |
| [IsReadOnly](../../aspose.tasks/availabilityperiodcollection/isreadonly/) { get; } | Restituisce un valore che indica se questa collezione è di sola lettura; altrimenti, false. |
| [Item](../../aspose.tasks/availabilityperiodcollection/item/) { get; set; } | Restituisce o imposta l'elemento all'indice specificato. |
| [ParentResource](../../aspose.tasks/availabilityperiodcollection/parentresource/) { get; } | Ottiene il [`Resource`](../resource/) genitore per questo oggetto. Oggetto [`Resource`](../resource/) genitore per questa collezione. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/availabilityperiodcollection/add/)(AvailabilityPeriod) | Aggiunge l'elemento specificato a questa collezione. |
| [Clear](../../aspose.tasks/availabilityperiodcollection/clear/)() | Rimuove tutti gli elementi da questa collezione. |
| [Contains](../../aspose.tasks/availabilityperiodcollection/contains/)(AvailabilityPeriod) | Restituisce true se l'elemento specificato è presente in questa collezione; altrimenti, false. |
| [CopyTo](../../aspose.tasks/availabilityperiodcollection/copyto/)(AvailabilityPeriod[], int) | Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato. |
| [GetEnumerator](../../aspose.tasks/availabilityperiodcollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [IndexOf](../../aspose.tasks/availabilityperiodcollection/indexof/)(AvailabilityPeriod) | Determina l'indice dell'elemento specificato in questa collezione. |
| [Insert](../../aspose.tasks/availabilityperiodcollection/insert/)(int, AvailabilityPeriod) | Inserisce l'elemento specificato all'indice specificato. |
| [Remove](../../aspose.tasks/availabilityperiodcollection/remove/)(AvailabilityPeriod) | Rimuove la prima occorrenza di un oggetto specifico da questa collezione. |
| [RemoveAt](../../aspose.tasks/availabilityperiodcollection/removeat/)(int) | Rimuove un elemento all'indice specificato. |

## Esempi

Mostra come lavorare con la collezione di periodi di disponibilità di una risorsa.

```csharp
public void WorkWithAvailabilityPeriodCollection()
{
    var project = new Project(DataDir + "UpdateResourceData.mpp");
    var resource = project.Resources.GetById(1);

    resource.AvailabilityPeriods.Clear();

    // Aggiungi periodi di disponibilità (anni 2012 e 2014) alla nuova risorsa
    IEnumerable<AvailabilityPeriod> periods = this.GetPeriods();
    foreach (var period in periods)
    {
        if (!resource.AvailabilityPeriods.IsReadOnly)
        {
            resource.AvailabilityPeriods.Add(period);
        }
    }

    var period2013 = new AvailabilityPeriod { AvailableFrom = new DateTime(2013, 1, 1), AvailableTo = new DateTime(2013, 12, 12), AvailableUnits = 0.81 };

    if (!resource.AvailabilityPeriods.Contains(period2013))
    {
        resource.AvailabilityPeriods.Insert(1, period2013);
    }

    Console.WriteLine("Count of availability periods: " + resource.AvailabilityPeriods.Count);
    foreach (var period in resource.AvailabilityPeriods)
    {
        Console.WriteLine("Available From: " + period.AvailableFrom);
        Console.WriteLine("Available To: " + period.AvailableTo);
        Console.WriteLine("Available Units: " + period.AvailableUnits);
        Console.WriteLine();
    }

    var periodsToCopy = new AvailabilityPeriod[resource.AvailabilityPeriods.Count];
    resource.AvailabilityPeriods.CopyTo(periodsToCopy, 0);

    var otherResource = project.Resources.GetById(2);
    otherResource.AvailabilityPeriods.Clear();
    foreach (var period in periodsToCopy)
    {
        otherResource.AvailabilityPeriods.Add(period);
    }

    var period2015 = new AvailabilityPeriod { AvailableFrom = new DateTime(2015, 1, 1), AvailableTo = new DateTime(2015, 12, 12), AvailableUnits = 0.50 };

    var period2016 = new AvailabilityPeriod { AvailableFrom = new DateTime(2016, 1, 1), AvailableTo = new DateTime(2016, 12, 12), AvailableUnits = 0.53 };

    if (otherResource.AvailabilityPeriods.IndexOf(period2015) < 0)
    {
        otherResource.AvailabilityPeriods.Add(period2015);
    }

    if (otherResource.AvailabilityPeriods.IndexOf(period2016) < 0)
    {
        otherResource.AvailabilityPeriods.Add(period2016);
    }

    // aggiorna le unità disponibili per il periodo dell'anno 2014
    otherResource.AvailabilityPeriods[otherResource.AvailabilityPeriods.Count - 2].AvailableUnits = 0.90;

    // rimuovi il periodo del 2013
    otherResource.AvailabilityPeriods.Remove(period2013);

    // rimuovi il periodo del 2011
    otherResource.AvailabilityPeriods.RemoveAt(0);

    Console.WriteLine("Print resource availability periods of the resource: " + otherResource.Get(Rsc.Name));
    Console.WriteLine("Count of availability periods: " + resource.AvailabilityPeriods.Count);
    foreach (var period in resource.AvailabilityPeriods)
    {
        Console.WriteLine("Available From: " + period.AvailableFrom);
        Console.WriteLine("Available To: " + period.AvailableTo);
        Console.WriteLine("Available Units: " + period.AvailableUnits);
        Console.WriteLine();
    }
}

private IEnumerable<AvailabilityPeriod> GetPeriods()
{
    var periods = new List<AvailabilityPeriod>();
    var period = new AvailabilityPeriod { AvailableFrom = new DateTime(2012, 1, 1), AvailableTo = new DateTime(2012, 12, 12), AvailableUnits = 0.99 };
    periods.Add(period);

    var period2 = new AvailabilityPeriod { AvailableFrom = new DateTime(2014, 1, 1), AvailableTo = new DateTime(2014, 12, 12), AvailableUnits = 0.94 };
    periods.Add(period2);
    return periods;
}
```

### Vedi anche

* class [AvailabilityPeriod](../availabilityperiod/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


