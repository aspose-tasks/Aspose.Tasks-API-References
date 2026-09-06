---
title: "Asn.Uid"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. المعرف الفريد لتعيين."
type: docs
weight: 560
url: /ar/net/aspose.tasks/asn/uid/
---
## Asn.Uid field

المعرّف الفريد للمهمة.

```csharp
public static readonly Key<int, AsnKey> Uid;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Asn.Uid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Uid, 30);

Console.WriteLine("UID: " + assignment.Get(Asn.Uid));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


