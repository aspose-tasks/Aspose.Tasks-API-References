---
title: "Asn.Summary"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. يحدد ما إذا كانت المهمة مهمة ملخصة"
type: docs
weight: 530
url: /ar/net/aspose.tasks/asn/summary/
---
## Asn.Summary field

يحدد ما إذا كانت المهمة مهمة ملخص.

```csharp
public static readonly Key<bool, AsnKey> Summary;
```

## الأمثلة

يظهر كيفية قراءة خاصية Asn.Summary.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Summary, true);

Console.WriteLine("Summary: " + assignment.Get(Asn.Summary));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


