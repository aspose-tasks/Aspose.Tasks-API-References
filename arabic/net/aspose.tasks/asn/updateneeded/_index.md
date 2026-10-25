---
title: "Asn.UpdateNeeded"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. يحدد ما إذا كان المورد المعين لمهمة يحتاج إلى تحديث وفقًا لحالة المهمة"
type: docs
weight: 580
url: /ar/net/aspose.tasks/asn/updateneeded/
---
## Asn.UpdateNeeded field

يحدد ما إذا كان يجب تحديث المورد المعين لمهمة وفقًا لحالة المهمة.

```csharp
public static readonly Key<bool, AsnKey> UpdateNeeded;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Asn.UpdateNeeded.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.UpdateNeeded, true);

Console.WriteLine("Update Needed: " + assignment.Get(Asn.UpdateNeeded));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


