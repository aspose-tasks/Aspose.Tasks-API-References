---
title: "Asn.VAC"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Asn field. الفرق بين التكلفة الأساسية والتكلفة الإجمالية"
type: docs
weight: 590
url: /ar/net/aspose.tasks/asn/vac/
---
## Asn.VAC field

الفرق بين التكلفة الأساسية والتكلفة الإجمالية.

```csharp
public static readonly Key<double, AsnKey> VAC;
```

## الأمثلة

يعرض كيفية قراءة خاصية Asn.VAC.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.VAC, 10);

Console.WriteLine("VAC: " + assignment.Get(Asn.VAC));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


