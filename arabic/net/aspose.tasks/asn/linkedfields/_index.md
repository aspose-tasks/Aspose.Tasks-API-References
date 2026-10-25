---
title: "Asn.LinkedFields"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. يحدد ما إذا كان المشروع مرتبطًا بكائن OLE آخر"
type: docs
weight: 320
url: /ar/net/aspose.tasks/asn/linkedfields/
---
## Asn.LinkedFields field

يحدد ما إذا كان المشروع مرتبطًا بكائن OLE آخر.

```csharp
public static readonly Key<bool, AsnKey> LinkedFields;
```

## الأمثلة

يعرض كيفية قراءة خاصية Asn.LinkedFields.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Linked Fields: " + assignment.Get(Asn.LinkedFields));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


