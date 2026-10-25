---
title: "Asn.Task"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. المهمة التي يتم تعيين مورد لها"
type: docs
weight: 550
url: /ar/net/aspose.tasks/asn/task/
---
## Asn.Task field

المهمة التي يُعيّن لها المورد.

```csharp
public static readonly Key<Task, AsnKey> Task;
```

## الأمثلة

يعرض كيفية قراءة خصائص Asn.Task و Asn.Resource.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assigned Task Name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
Console.WriteLine("Assigned Resource Name: " + assignment.Get(Asn.Resource).Get(Rsc.Name));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Task](../../task/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


