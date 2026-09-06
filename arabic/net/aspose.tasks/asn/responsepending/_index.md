---
title: "Asn.ResponsePending"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Asn field. يحدد ما إذا تم استلام الرد لرسالة TeamAssign"
type: docs
weight: 480
url: /ar/net/aspose.tasks/asn/responsepending/
---
## Asn.ResponsePending field

يحدد ما إذا تم استلام الاستجابة لرسالة TeamAssign.

```csharp
public static readonly Key<bool, AsnKey> ResponsePending;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Asn.ResponsePending.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.ResponsePending, true);

Console.WriteLine("Response Pending: " + assignment.Get(Asn.ResponsePending));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


