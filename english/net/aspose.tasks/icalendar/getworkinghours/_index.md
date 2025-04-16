---
title: ICalendar.GetWorkingHours
second_title: Aspose.Tasks for .NET API Reference
description: ICalendar method. Return WorkUnit  Start Finish and Duration of working hours for the specified date time interval
type: docs
weight: 60
url: /net/aspose.tasks/icalendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Return WorkUnit - Start, Finish and Duration of working hours for the specified date time interval.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | Start date of the interval. |
| finish | DateTime | Finish date of the interval. |

### Return Value

Instance of [`WorkUnit`](../../workunit/) class containing Start, Finish and Duration of working hours.

### See Also

* class [WorkUnit](../../workunit/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Returns the amount of working hours at the specified date.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dt | DateTime | The date to get working hours for. |

### Return Value

Working hours at the specified date.

### See Also

* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


