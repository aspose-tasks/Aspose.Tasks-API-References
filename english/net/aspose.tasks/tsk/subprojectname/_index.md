---
title: Tsk.SubprojectName
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The source location of a subproject
type: docs
weight: 1070
url: /net/aspose.tasks/tsk/subprojectname/
---
## Tsk.SubprojectName field

The source location of a subproject.

```csharp
public static readonly Key<string, TaskKey> SubprojectName;
```

## Examples

Shows how to create a subproject task.

```csharp
var project = new Project(DataDir + "SubProjectTask.mpp");

// Add task
var task = project.RootTask.Children.Add("Task 1");

// Setting new subproject link
task.Set(Tsk.SubprojectName, DataDir + "subProject.mpp");

project.Save(OutDir + "CreateSubProjectTask_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


