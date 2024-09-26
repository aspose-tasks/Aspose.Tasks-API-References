---
title: Tsk.ActivityId
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Represents activity id field  a tasks unique identifier used by Primavera. only applicable to Primavera projects
type: docs
weight: 10
url: /net/aspose.tasks/tsk/activityid/
---
## Tsk.ActivityId field

Represents activity id field - a task's unique identifier used by Primavera. (only applicable to Primavera projects).

```csharp
public static readonly Key<string, TaskKey> ActivityId;
```

## Examples

Shows how to work with ActivityId field specific to Primavera projects

```csharp
var project = new Project(DataDir + "test.xer");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Task activity_id: {0}", task.Get(Tsk.ActivityId));

task.Set(Tsk.ActivityId, "CUSTOM_ACTIVITY_ID");

// create Primavera save options and specify that ActivityIds should not be overwritten during saving.
var options = new PrimaveraSaveOptions
{
    RenumberActivityIds = false
};

project.Save(OutDir + "WorkWithPrimaveraActivityId_out.xer", options);
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


