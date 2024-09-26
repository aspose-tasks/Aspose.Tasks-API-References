---
title: Tsk.Contact
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The name of an individual responsible for a task
type: docs
weight: 220
url: /net/aspose.tasks/tsk/contact/
---
## Tsk.Contact field

The name of an individual responsible for a task.

```csharp
public static readonly Key<string, TaskKey> Contact;
```

## Examples

Shows how to read/write Tsk.Contact property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Contact, "John Smith");

Console.WriteLine("Contact: " + task.Get(Tsk.Contact));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


