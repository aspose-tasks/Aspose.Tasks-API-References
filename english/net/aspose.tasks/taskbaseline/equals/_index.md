---
title: TaskBaseline.Equals
second_title: Aspose.Tasks for .NET API Reference
description: TaskBaseline method. Returns a value indicating whether this instance is equal to the specified TaskBaseline object
type: docs
weight: 100
url: /net/aspose.tasks/taskbaseline/equals/
---
## Equals(TaskBaseline) {#equals_1}

Returns a value indicating whether this instance is equal to the specified TaskBaseline object.

```csharp
public bool Equals(TaskBaseline other)
```

| Parameter | Type | Description |
| --- | --- | --- |
| other | TaskBaseline | the specified AssignmentBaseline object to compare with this instance. |

### Return Value

returns true if this instance is equal to the specified TaskBaseline object; otherwise, false.

## Examples

Shows how to check equality of baselines.

```csharp
var project = new Project();

// creating TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// display task baseline duration
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// the equality of baselines is checked against to baseline's numbers.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### See Also

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_2}

Returns a value indicating whether this instance is equal to a specified object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The object to compare with this instance. |

### Return Value

**True** if the specified object is a TaskBaseline that has the same UID value as this instance; otherwise, **false**.

## Examples

Shows how to check equality of baselines.

```csharp
var project = new Project();

// creating TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// display task baseline duration
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// the equality of baselines is checked against to baseline's numbers.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### See Also

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


