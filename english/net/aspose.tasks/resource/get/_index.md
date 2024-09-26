---
title: Resource.Get
second_title: Aspose.Tasks for .NET API Reference
description: Resource method. Returns the value to which the property is mapped in this container
type: docs
weight: 830
url: /net/aspose.tasks/resource/get/
---
## Resource.Get&lt;T&gt; method

Returns the value to which the property is mapped in this container.

```csharp
public T Get<T>(Key<T, RscKey> key)
```

| Parameter | Description |
| --- | --- |
| T | the type of the mapped value. |
| key | the specified property key. [`Rsc`](../../rsc/) for getting the property key. |

### Return Value

the value to which the property is mapped in this container.

## Examples

Shows how to read/write common resource properties.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// Add resource and set some properties
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


