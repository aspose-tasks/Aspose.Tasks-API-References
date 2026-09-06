---
title: "Asn.Milestone"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. يحدد ما إذا كان التعيين علامة إنجاز"
type: docs
weight: 330
url: /ar/net/aspose.tasks/asn/milestone/
---
## Asn.Milestone field

يحدد ما إذا كانت المهمة علامةً رئيسية.

```csharp
public static readonly Key<bool, AsnKey> Milestone;
```

## الأمثلة

يعرض كيفية قراءة خاصية Asn.Milestone.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Milestone: " + assignment.Get(Asn.Milestone));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


