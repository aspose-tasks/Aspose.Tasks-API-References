---
title: Filter.CompareTo
second_title: Aspose.Tasks for .NET API Reference
description: Filter method. Compares this instance to the specified instance of the Filter class and returns an indication of their relative order
type: docs
weight: 90
url: /net/aspose.tasks/filter/compareto/
---
## Filter.CompareTo method

Compares this instance to the specified instance of the [`Filter`](../) class and returns an indication of their relative order.

```csharp
public int CompareTo(Filter other)
```

| Parameter | Type | Description |
| --- | --- | --- |
| other | Filter | the specified instance of the [`Filter`](../) class to compare to this object. |

### Return Value

an indication of their relative order.

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


