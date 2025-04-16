---
title: Task.GetTimephasedData
second_title: Aspose.Tasks for .NET API Reference
description: Task method. Returns TimephasedDataCollection object with TimephasedData values within given start and end dates of specified timephased data type
type: docs
weight: 1360
url: /net/aspose.tasks/task/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Returns [`TimephasedDataCollection`](../../timephaseddatacollection/) object with [`TimephasedData`](../timephaseddata/) values within given start and end dates of specified time-phased data type.

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

A [`TimephasedDataCollection`](../../timephaseddatacollection/) object with [`TimephasedData`](../timephaseddata/) values within given start and end dates of specified timephased data type.

## Examples

Shows how to get timephased data (with specific type) of the task.

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

### See Also

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Returns [`TimephasedDataCollection`](../../timephaseddatacollection/) object with [`TimephasedData`](../timephaseddata/) values within given start and end dates.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | The start date for the time phased data. |
| end | DateTime | The end date for the time phased data. |

### Return Value

List of [`TimephasedData`](../../timephaseddata/) to be filled in.

## Examples

Shows how to get timephased data (with TaskWork type) of the task.

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

### See Also

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


