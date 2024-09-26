---
title: Prj.WorkFormat
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The format used to show the duration of the task
type: docs
weight: 790
url: /net/aspose.tasks/prj/workformat/
---
## Prj.WorkFormat field

The format used to show the duration of the task.

```csharp
public static readonly Key<TimeUnitType, PrjKey> WorkFormat;
```

## Examples

Shows how to get a duration with default work format.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// create a work value with project's default work format
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


