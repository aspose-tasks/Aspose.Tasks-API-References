---
title: Calendar.GetStartDateFromFinishAndDuration
second_title: Aspose.Tasks for .NET API Reference
description: Calendar method. Returns start date based on the specified finish date and duration
type: docs
weight: 200
url: /net/aspose.tasks/calendar/getstartdatefromfinishandduration/
---
## GetStartDateFromFinishAndDuration(DateTime, Duration) {#getstartdatefromfinishandduration}

Returns start date based on the specified finish date and duration.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, Duration duration)
```

| Parameter | Type | Description |
| --- | --- | --- |
| finish | DateTime | The specified finish date. |
| duration | Duration | The specified duration. |

### Return Value

Calculated start date.

## Examples

Shows how to get a start date by finish date and duration.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// get start date by finish date and a duration
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), project.GetDuration(16, TimeUnitType.Hour));

// 8 April 2020 9:00 AM will be printed
Console.WriteLine(startDate);
```

### See Also

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetStartDateFromFinishAndDuration(DateTime, TimeSpan) {#getstartdatefromfinishandduration_1}

Returns start date based on specified finish date and duration.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, TimeSpan duration)
```

| Parameter | Type | Description |
| --- | --- | --- |
| finish | DateTime | The specified finish date. |
| duration | TimeSpan | The specified duration. |

### Return Value

Calculated start date.

## Examples

Shows how to get a start date by finish date and duration (as a time span).

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// get start date by finish date and a duration
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), TimeSpan.FromHours(16));

// 8 April 2020 9:00 AM will be printed
Console.WriteLine(startDate);
```

### See Also

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


