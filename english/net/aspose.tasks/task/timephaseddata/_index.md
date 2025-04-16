---
title: Task.TimephasedData
second_title: Aspose.Tasks for .NET API Reference
description: Task property. Gets or sets a TimephasedDataCollection object of this task. The time phased data block associated with a task
type: docs
weight: 1220
url: /net/aspose.tasks/task/timephaseddata/
---
## Task.TimephasedData property

Gets or sets a TimephasedDataCollection object of this task. The time phased data block associated with a task.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Remarks

Reading supported for XML format only.

## Examples

Shows how to iterate over task's timephased data.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

foreach (var td in task.TimephasedData)
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


