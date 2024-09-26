---
title: Tsk.IsSubprojectReadOnly
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether a subproject is readonly
type: docs
weight: 710
url: /net/aspose.tasks/tsk/issubprojectreadonly/
---
## Tsk.IsSubprojectReadOnly field

Determines whether a subproject is read-only.

```csharp
public static readonly Key<NullableBool, TaskKey> IsSubprojectReadOnly;
```

## Examples

Shows how to read/write Tsk.IsSubprojectReadOnly property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubprojectReadOnly, true);

Console.WriteLine("Is Subproject Read Only: " + task.Get(Tsk.IsSubprojectReadOnly));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


