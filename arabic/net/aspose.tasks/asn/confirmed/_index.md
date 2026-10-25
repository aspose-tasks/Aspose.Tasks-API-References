---
title: "Asn.Confirmed"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. يحدد ما إذا كان المورد قد قبل جميع تعييناته"
type: docs
weight: 170
url: /ar/net/aspose.tasks/asn/confirmed/
---
## Asn.Confirmed field

يحدد ما إذا كان المورد قد قبل جميع مهامه.

```csharp
public static readonly Key<bool, AsnKey> Confirmed;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Asn.Confirmed.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Confirmed, true);

Console.WriteLine("Confirmed: " + assignment.Get(Asn.Confirmed));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


