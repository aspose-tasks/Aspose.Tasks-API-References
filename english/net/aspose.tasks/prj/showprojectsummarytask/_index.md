---
title: Prj.ShowProjectSummaryTask
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether to display summary information about an entire project on a single row with its own summary task bar at the top of the Gantt Chart view
type: docs
weight: 640
url: /net/aspose.tasks/prj/showprojectsummarytask/
---
## Prj.ShowProjectSummaryTask field

Determines whether to display summary information about an entire project on a single row with its own summary task bar at the top of the Gantt Chart view.

```csharp
public static readonly Key<bool, PrjKey> ShowProjectSummaryTask;
```

## Examples

Shows how to read/write Prj.ShowProjectSummaryTask property.

```csharp
var project = new Project();

project.Set(Prj.ShowProjectSummaryTask, true);

Console.WriteLine("Show Project Summary Task: " + project.Get(Prj.ShowProjectSummaryTask));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


