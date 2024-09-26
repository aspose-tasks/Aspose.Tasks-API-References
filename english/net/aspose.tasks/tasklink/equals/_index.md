---
title: TaskLink.Equals
second_title: Aspose.Tasks for .NET API Reference
description: TaskLink method. Returns a value indicating whether this instance is equal to a specified object
type: docs
weight: 90
url: /net/aspose.tasks/tasklink/equals/
---
## Equals(TaskLink) {#equals}

Returns a value indicating whether this instance is equal to a specified object.

```csharp
public bool Equals(TaskLink other)
```

| Parameter | Type | Description |
| --- | --- | --- |
| other | TaskLink | The specified instance of the [`TaskLink`](../) class to compare with this instance. |

### Return Value

**True** if the specified instance of the [`TaskLink`](../) class has the same predecessor and successor tasks as this instance; otherwise, **false**.

## Examples

Shows how to check equality of task links.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// the equality of task links is based on pred and succ tasks.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### See Also

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Returns a value indicating whether this instance is equal to a specified object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The object to compare with this instance. |

### Return Value

**True** if the specified object is a TaskLink that has the same predecessor and successor as this instance; otherwise, **false**.

## Examples

Shows how to check equality of task links.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// the equality of task links is based on pred and succ tasks.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### See Also

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


