---
title: Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether manual tasks must be kept on nearest working time when made as auto scheduled
type: docs
weight: 400
url: /net/aspose.tasks/prj/keeptaskonnearestworkingtimewhenmadeautoscheduled/
---
## Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled field

Determines whether manual tasks must be kept on nearest working time when made as auto scheduled.

```csharp
public static readonly Key<NullableBool, PrjKey> KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled;
```

## Examples

Shows how to read/write Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled property.

```csharp
var project = new Project();

project.Set(Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled, true);

Console.WriteLine("Keep Task On Nearest Working Time When Made Auto Scheduled: " + project.Get(Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


