---
title: ResourceAssignment.GetTimephasedWork
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment method. Gets amount of timephased work for the specified date time interval
type: docs
weight: 730
url: /net/aspose.tasks/resourceassignment/gettimephasedwork/
---
## GetTimephasedWork(DateTime, DateTime, TimephasedDataType) {#gettimephasedwork_1}

Gets amount of timephased work for the specified date time interval.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end, 
    TimephasedDataType timephasedDataType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | Start of the date time interval. |
| end | DateTime | End of the date time interval. |
| timephasedDataType | TimephasedDataType | Type of the timephased data to use. |

## Examples

Shows how to calculate assignment's work for arbitrary date time interval.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var assignment = project.ResourceAssignments.GetByUid(2);

// Print assignmen's work for each hour.
for (DateTime hour = assignment.Start; hour <= assignment.Finish; hour = hour.AddHours(1))
{
    var work = assignment.GetTimephasedWork(hour, hour.AddHours(1), TimephasedDataType.AssignmentWork);
    Console.WriteLine("{0} : {1:N2}", hour, work.TotalHours);
}
```

### See Also

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedWork(DateTime, DateTime) {#gettimephasedwork}

Gets amount of timephased work for the specified date time interval.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | Start of the date time interval. |
| end | DateTime | End of the date time interval. |

### See Also

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


