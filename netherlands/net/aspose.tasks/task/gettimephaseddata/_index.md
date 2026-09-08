---
title: "Task.GetTimephasedData"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task-methode. Retourneert een TimephasedDataCollection-object met TimephasedData-waarden binnen de opgegeven start- en einddatums van het gespecificeerde timephased-gegevens type"
type: docs
weight: 1360
url: /nl/net/aspose.tasks/task/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Retourneert [`TimephasedDataCollection`](../../timephaseddatacollection/) object met [`TimephasedData`](../timephaseddata/) waarden binnen de opgegeven start- en einddatums van het gespecificeerde time‑phased-gegevens type.

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

Een [`TimephasedDataCollection`](../../timephaseddatacollection/) object met [`TimephasedData`](../timephaseddata/) waarden binnen de opgegeven start- en einddatums van het gespecificeerde timephased-gegevens type.

## Voorbeelden

Toont hoe timephased-gegevens (met een specifiek type) van de taak op te halen.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate).AddDays(2), TimephasedDataType.TaskBaselineWork)
    .ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### Zie ook

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Retourneert [`TimephasedDataCollection`](../../timephaseddatacollection/) object met [`TimephasedData`](../timephaseddata/) waarden binnen de opgegeven start- en einddatums.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | DateTime | De startdatum voor de tijdgephaseerde gegevens. |
| einde | DateTime | De einddatum voor de tijdgephaseerde gegevens. |

### Retourwaarde

Lijst van [`TimephasedData`](../../timephaseddata/) die moet worden ingevuld.

## Voorbeelden

Toont hoe u tijdgephaseerde gegevens (met type TaskWork) van de taak kunt ophalen.

```csharp
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)).ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### Zie ook

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


