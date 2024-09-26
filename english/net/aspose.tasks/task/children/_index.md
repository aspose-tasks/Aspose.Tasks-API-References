---
title: Task.Children
second_title: Aspose.Tasks for .NET API Reference
description: Task property. Gets a child task collection of this object. TaskCollection object which represents children tasks
type: docs
weight: 190
url: /net/aspose.tasks/task/children/
---
## Task.Children property

Gets a child task collection of this object. TaskCollection object which represents children tasks.

```csharp
public TaskCollection Children { get; }
```

## Examples

Shows how to use task collection to add a task.

```csharp
var project = new Project();

// Add task, sub task and save project
var task = project.RootTask.Children.Add("Summary1");
task.Children.Add("Subtask1");
project.Save(OutDir + "CreateTasks_out.xml", SaveFileFormat.Xml);
```

### See Also

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


