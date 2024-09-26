---
title: Project.GetDuration
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Gets Duration object with the specified number of units and default duration format which is defined in projects settings DurationFormat
type: docs
weight: 1090
url: /net/aspose.tasks/project/getduration/
---
## GetDuration(double) {#getduration}

Gets [`Duration`](../../duration/) object with the specified number of units and default duration format which is defined in project's settings [`DurationFormat`](../../prj/durationformat/).

```csharp
public Duration GetDuration(double val)
```

| Parameter | Type | Description |
| --- | --- | --- |
| val | Double | specified number of units. |

### Return Value

Duration object.

## Remarks

This method should be used carefully because it returns different durations depending on Project.DurationFormat setting. For example, GetWork(1.0) will return 1 hour when Project.DurationFormat is TimeUnitType.Hour or 1 day if Project.DurationFormat is TimeUnitType.Day.

## Examples

Shows how to create a &lt;see cref="Aspose.Tasks.Duration" /&gt; instance with default project's duration format by using project fabric methods.

```csharp
var project = new Project();

// get a duration with default project format.
var duration = project.GetDuration(1);

Console.WriteLine("Default project duration time unit type: " + project.Get(Prj.DurationFormat));
Console.WriteLine("Created duration time unit type: " + duration.TimeUnit);
```

### See Also

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(double, TimeUnitType) {#getduration_1}

Gets [`Duration`](../../duration/) object with the specified number of [`TimeUnitType`](../../timeunittype/) units.

```csharp
public Duration GetDuration(double val, TimeUnitType timeUnit)
```

| Parameter | Type | Description |
| --- | --- | --- |
| val | Double | specified number of units. |
| timeUnit | TimeUnitType | specified TimeUnitType value. |

### Return Value

Duration object.

## Examples

Shows how to create a &lt;see cref="Aspose.Tasks.Duration" /&gt; instance by using project fabric methods.

```csharp
var project = new Project();

// get a duration with default project format.
var duration = project.GetDuration(1, TimeUnitType.Minute);

Console.WriteLine("Created duration: " + duration);
```

### See Also

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(TimeSpan, TimeUnitType) {#getduration_2}

Gets [`Duration`](../../duration/) object with the specified TimeSpan value and specified [`TimeUnitType`](../../timeunittype/) value.

```csharp
public Duration GetDuration(TimeSpan timeSpan, TimeUnitType timeUnit)
```

| Parameter | Type | Description |
| --- | --- | --- |
| timeSpan | TimeSpan | specified TimeSpan value. |
| timeUnit | TimeUnitType | specified TimeUnitType value. |

### Return Value

Duration object.

### See Also

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


