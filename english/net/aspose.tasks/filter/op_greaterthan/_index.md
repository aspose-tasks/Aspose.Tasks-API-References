---
title: Filter.op_GreaterThan
second_title: Aspose.Tasks for .NET API Reference
description: Filter method. Returns a value indicating whether this instance is greater than a specified object
type: docs
weight: 130
url: /net/aspose.tasks/filter/op_greaterthan/
---
## Filter GreaterThan operator

Returns a value indicating whether this instance is greater than a specified object.

```csharp
public static bool operator >(Filter a, Filter b)
```

| Parameter | Type | Description |
| --- | --- | --- |
| a | Filter | The first filter. |
| b | Filter | The second filter. |

### Return Value

a value indicating whether this instance is greater than a specified object

## Examples

Shows how to check filter equality.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();

var filter1 = filters[0];
var filter2 = filters[1];

// the equality of filters is checked against to filter's UID.
Console.WriteLine("Filter 1 UID: " + filter1.Uid);
Console.WriteLine("Filter 2 UID: " + filter2.Uid);
Console.WriteLine("Are filters equal: " + filter1.Equals(filter2));
```

### See Also

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


