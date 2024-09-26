---
title: Filter.Equals
second_title: Aspose.Tasks for .NET API Reference
description: Filter method. Returns a value indicating whether this instance is equal to the specified AssignmentBaseline object
type: docs
weight: 100
url: /net/aspose.tasks/filter/equals/
---
## Equals(Filter) {#equals}

Returns a value indicating whether this instance is equal to the specified AssignmentBaseline object.

```csharp
public bool Equals(Filter other)
```

| Parameter | Type | Description |
| --- | --- | --- |
| other | Filter | the specified AssignmentBaseline object to compare with this instance. |

### Return Value

returns true if this instance is equal to the specified AssignmentBaseline object; otherwise, false.

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

---

## Equals(object) {#equals_1}

Returns a value indicating whether this instance is equal to the specified AssignmentBaseline object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | the specified AssignmentBaseline object to compare with this instance. |

### Return Value

returns true if this instance is equal to the specified AssignmentBaseline object; otherwise, false.

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


