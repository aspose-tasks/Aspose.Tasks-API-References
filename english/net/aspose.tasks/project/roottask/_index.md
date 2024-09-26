---
title: Project.RootTask
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets the root of the tree of tasks
type: docs
weight: 790
url: /net/aspose.tasks/project/roottask/
---
## Project.RootTask property

Gets the root of the tree of tasks.

```csharp
public Task RootTask { get; }
```

## Examples

Shows how to add a task into a project by using the root project task.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddNewTask_out.xml", SaveFileFormat.Xml);
```

### See Also

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


