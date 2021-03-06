---
title: RescheduleUncompletedWorkToStartAfter
second_title: Aspose.Tasks for .NET API Reference
description: 
type: docs
weight: 390
url: /net/aspose.tasks/project/rescheduleuncompletedworktostartafter/
---
## Project.RescheduleUncompletedWorkToStartAfter method (1 of 2)

Reschedules uncompleted project work to start after a specified date.

```csharp
public void RescheduleUncompletedWorkToStartAfter(DateTime after)
```

| Parameter | Type | Description |
| --- | --- | --- |
| after | DateTime | The date to reschedule uncompleted work after. |

### Remarks

Ensure that Project.CanSplitsInProgressTasks flag is set to true before using this method.

### See Also

* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project.RescheduleUncompletedWorkToStartAfter method (2 of 2)

Reschedules uncompleted work for a specified list of tasks to start after a specified date.

```csharp
public void RescheduleUncompletedWorkToStartAfter(DateTime after, List<Task> taskCollection)
```

| Parameter | Type | Description |
| --- | --- | --- |
| after | DateTime | The date to reschedule uncompleted work after. |
| taskCollection | List`1 | List&lt;Task&gt; of tasks to reschedule uncompleted work for. |

### Remarks

Ensure that Project.CanSplitsInProgressTasks flag is set to true before using this method.

### See Also

* class [Task](../../task)
* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
