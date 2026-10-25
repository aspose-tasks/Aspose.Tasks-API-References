---
title: "Resource.GetTimephasedData"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Resource-methode. Retourneert een instantie van de TimephasedDataCollection-klasse voor dit object met de TimephasedData-waarden binnen de opgegeven start- en einddatums van het opgegeven TimephasedDataType"
type: docs
weight: 850
url: /nl/net/aspose.tasks/resource/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Retourneert een instantie van de [`TimephasedDataCollection`](../../timephaseddatacollection/) klasse voor dit object met de [`TimephasedData`](../timephaseddata/) waarden binnen de opgegeven start- en einddatums van het opgegeven [`TimephasedDataType`](../../timephaseddatatype/).

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | DateTime | De startdatum voor de tijdgephaseerde gegevens. |
| einde | DateTime | De einddatum voor de tijdgephaseerde gegevens. |
| timephasedType | TimephasedDataType | Het type tijdgephaseerde gegevens ([`TimephasedDataType`](../../timephaseddatatype/)). |

### Retourwaarde

Lijst van [`TimephasedData`](../timephaseddata/).

## Voorbeelden

Toont hoe tijdgephaseerde gegevens van werk-/kostenbronnen gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Haal de Resource op via zijn ID
var resource = project.Resources.GetByUid(1);

// Print tijdgephaseerde gegevens van ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// Print tijdgephaseerde gegevens van ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### Zie ook

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Retourneert [`TimephasedDataCollection`](../../timephaseddatacollection/) voor dit object met [`TimephasedData`](../timephaseddata/) waarden binnen de opgegeven start- en einddatums.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | DateTime | De startdatum voor de tijdgephaseerde gegevens. |
| einde | DateTime | De einddatum voor de tijdgephaseerde gegevens. |

### Retourwaarde

Lijst van [`TimephasedData`](../../timephaseddata/).

## Voorbeelden

Toont hoe tijdgephaseerde gegevens van werk-/kostenbronnen gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Haal de Resource op via zijn ID
var resource = project.Resources.GetByUid(1);

// Print tijdgephaseerde gegevens van ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// Print tijdgephaseerde gegevens van ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### Zie ook

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


