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
foreach (var td in resource.TimephasedData)
{
    Console.WriteLine(td.Start);
    Console.WriteLine(td.Finish);
}
```

### See Also

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


