---
title: Resource.TimephasedData
second_title: Aspose.Tasks for .NET API Reference
description: Resource property. Gets or sets an instance of TimephasedDataCollection class for this object
type: docs
weight: 740
url: /net/aspose.tasks/resource/timephaseddata/
---
## Resource.TimephasedData property

Gets or sets an instance of [`TimephasedDataCollection`](../../timephaseddatacollection/) class for this object.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Remarks

Reading supported for XML format only.

## Examples

Shows how to read resource timephased data.

```csharp
resource.Set(Rsc.Work, resource.ParentProject.GetWork(2));

project.SetBaseline(BaselineType.Baseline);

// iterate over timephased data of the resource
Console.WriteLine("Regular work timephased data: ");
foreach (var td in resource.GetTimephasedData(task.Start, task.Finish, TimephasedDataType.ResourceWork))
{
    Console.WriteLine("[{0}] {1} - {2}, {3}", td.TimephasedDataType, td.Start, td.Finish, td.Value);
}

Console.WriteLine("Regular cost timephased data: ");
foreach (var td in resource.GetTimephasedData(task.Start, task.Finish, TimephasedDataType.ResourceCost))
{
    Console.WriteLine("[{0}] {1} - {2}, {3}", td.TimephasedDataType, td.Start, td.Finish, td.Value);
}

Console.WriteLine("Baseline timephased data: ");
foreach (var td in resource.Baselines[0].TimephasedData)
{
    Console.WriteLine("[{0}] {1} - {2}, {3}", td.TimephasedDataType, td.Start, td.Finish, td.Value);
}
```

### See Also

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


