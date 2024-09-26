---
title: Resource.GetTimephasedData
second_title: Aspose.Tasks for .NET API Reference
description: Resource method. Returns an instance of the TimephasedDataCollection class for this object with the TimephasedData values within given start and end dates of specified TimephasedDataType
type: docs
weight: 850
url: /net/aspose.tasks/resource/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Returns an instance of the [`TimephasedDataCollection`](../../timephaseddatacollection/) class for this object with the [`TimephasedData`](../timephaseddata/) values within given start and end dates of specified [`TimephasedDataType`](../../timephaseddatatype/).

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | The start date for the time phased data. |
| end | DateTime | The end date for the time phased data. |
| timephasedType | TimephasedDataType | The type of time phased data ([`TimephasedDataType`](../../timephaseddatatype/)). |

### Return Value

List of [`TimephasedData`](../timephaseddata/).

## Examples

Shows how to read timephased data of work/cost resources.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Get the Resource by its ID
var resource = project.Resources.GetByUid(1);

// Print Timephased data of ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// Print Timephased data of ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### See Also

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Returns [`TimephasedDataCollection`](../../timephaseddatacollection/) for this object with [`TimephasedData`](../timephaseddata/)values within given start and end dates.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | The start date for the time phased data. |
| end | DateTime | The end date for the time phased data. |

### Return Value

List of [`TimephasedData`](../../timephaseddata/).

## Examples

Shows how to read timephased data of work/cost resources.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Get the Resource by its ID
var resource = project.Resources.GetByUid(1);

// Print Timephased data of ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// Print Timephased data of ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### See Also

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


