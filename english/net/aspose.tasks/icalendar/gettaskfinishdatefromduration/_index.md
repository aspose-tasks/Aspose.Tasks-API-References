---
title: ICalendar.GetTaskFinishDateFromDuration
second_title: Aspose.Tasks for .NET API Reference
description: ICalendar method. Calculates the task finish date and time from its start date split parts and the work duration
type: docs
weight: 50
url: /net/aspose.tasks/icalendar/gettaskfinishdatefromduration/
---
## ICalendar.GetTaskFinishDateFromDuration method

Calculates the task finish date and time from its start date, split parts and the work duration.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Parameter | Type | Description |
| --- | --- | --- |
| task | Task | The task to calculate finish date for. |
| duration | TimeSpan | The duration to calculate. |

### Return Value

Task's finish date for the given start date and duration.

## Remarks

Returns DateTime.MinValue if task is summary, null or its start date is not set.

### See Also

* class [Task](../../task/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


