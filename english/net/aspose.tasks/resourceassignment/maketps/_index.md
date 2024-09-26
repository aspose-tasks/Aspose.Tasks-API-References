---
title: ResourceAssignment.MakeTPs
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment method. Generates a list of time phased data
type: docs
weight: 740
url: /net/aspose.tasks/resourceassignment/maketps/
---
## ResourceAssignment.MakeTPs method

Generates a list of time phased data.

```csharp
public DateTime MakeTPs(DateTime start, TimeSpan time, Calendar calendar, 
    List<TimephasedData> list, bool isWorking, int type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | The specified start date. |
| time | TimeSpan | The specified working time. |
| calendar | Calendar | The specified working calendar. |
| list | List`1 | The list of time phased data. |
| isWorking | Boolean | The specified flag which specifies whether time-phased data is working or not. |
| type | Int32 | The specified time-phased data type. |

### Return Value

A maximum date from list or start date if list is empty.

## Examples

Shows how to generate TPs by parameters.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 3, 30, 8, 0, 0));
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2020, 4, 1, 8, 0, 0));

var tps = new List<TimephasedData>();
var lastDate = assignment.MakeTPs(
    assignment.Get(Asn.Start),
    TimeSpan.FromHours(32),
    project.Calendars.GetByName("Standard"),
    tps,
    true,
    (int)TimephasedDataType.AssignmentRemainingWork);

foreach (var data in tps)
{
    Console.WriteLine("Start: " + data.Start);
    Console.WriteLine("Finish: " + data.Finish);
    Console.WriteLine("TimephasedDataType: " + data.TimephasedDataType);
    Console.WriteLine();
}
```

### See Also

* class [Calendar](../../calendar/)
* class [TimephasedData](../../timephaseddata/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


