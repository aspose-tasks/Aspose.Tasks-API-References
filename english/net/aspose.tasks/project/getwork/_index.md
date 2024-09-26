---
title: Project.GetWork
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Gets Duration object with the specified Double value and default work format
type: docs
weight: 1120
url: /net/aspose.tasks/project/getwork/
---
## Project.GetWork method

Gets [`Duration`](../../duration/) object with the specified Double value and default work format.

```csharp
public Duration GetWork(double val)
```

| Parameter | Type | Description |
| --- | --- | --- |
| val | Double | specified double value. |

### Return Value

Duration object.

## Remarks

This method should be used carefully because it returns different durations depending on Project.WorkFormat setting. For example, GetWork(1.0) will return 1 hour when Project.WorkFormat is TimeUnitType.Hour or 1 day if Project.WorkFormat is TimeUnitType.Day.

## Examples

Shows how to get a work with default work format.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// create a work value with project's default work format
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### See Also

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


