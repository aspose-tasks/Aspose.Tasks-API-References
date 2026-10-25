---
title: "Class RateCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.RateCollection class. Representa una colección que contiene objetos Rate"
type: docs
weight: 1630
url: /es/net/aspose.tasks/ratecollection/
---
## RateCollection class

Representa una colección que contiene objetos [`Rate`](../rate/).

```csharp
public class RateCollection : IDictionary<RateType, RateByDateCollection>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/ratecollection/count/) { get; } | Obtiene el número de elementos contenidos en RateCollection. |
| [IsReadOnly](../../aspose.tasks/ratecollection/isreadonly/) { get; } | Obtiene un valor que indica si esta colección es de solo lectura. |
| [Item](../../aspose.tasks/ratecollection/item/) { get; set; } | Devuelve o establece el elemento en el índice especificado. |
| [ParentResource](../../aspose.tasks/ratecollection/parentresource/) { get; } | Obtiene el objeto padre [`Resource`](../resource/) de esta colección. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/ratecollection/add/#add)(DateTime) | Agrega una nueva instancia de [`Rate`](../rate/) a esta colección. |
| [Add](../../aspose.tasks/ratecollection/add/#add_1)(DateTime, RateType) | Agrega una nueva instancia de [`Rate`](../rate/) a esta colección. |
| [GetEnumerator](../../aspose.tasks/ratecollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Remove](../../aspose.tasks/ratecollection/remove/)(Rate) | Elimina la instancia de Rate de esta colección. |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist)() | Convierte el objeto `RateCollection` en una lista de objetos [`Rate`](../rate/). |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist_1)(RateType) | Convierte el objeto `RateCollection` en una lista de objetos [`Rate`](../rate/) filtrados por el tipo [`RateType`](../ratetype/) especificado. |

## Ejemplos

Muestra cómo trabajar con colecciones de tasas.

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

// obtén la última tasa mediante acceso por índice
var rateToUpdate = resource.Rates[RateType.B][new DateTime(2019, 11, 12, 8, 0, 0)];
rateToUpdate.RatesTo = new DateTime(2020, 12, 31, 17, 0, 0);
Console.WriteLine("Rates From: " + rateToUpdate.RatesFrom);
Console.WriteLine("Rates To: " + rateToUpdate.RatesTo);

// ...
// trabaja con tasas
// ...

// elimina todas las tasas del tipo A
List<Rate> rates = resource.Rates.ToList(RateType.A);
for (var i = 0; i < rates.Count; i++)
{
    var rateToRemove = rates[i];
    resource.Rates.Remove(rateToRemove);
}

// transforma la colección de tasas en una lista plana
Console.WriteLine("Iterate over the rates after remove the A-typed values: ");
List<Rate> list = resource.Rates.ToList();
foreach (var rt in list)
{
    Console.WriteLine("Rates From: " + rt.RatesFrom);
    Console.WriteLine("Rates To: " + rt.RatesTo);
    Console.WriteLine("Rate Table: " + rt.RateTable);
}
```

### Ver también

* enum [RateType](../ratetype/)
* class [RateByDateCollection](../ratebydatecollection/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


