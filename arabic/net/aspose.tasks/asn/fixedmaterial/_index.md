---
title: "Asn.FixedMaterial"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. يحدد ما إذا كان استهلاك المورد المادي المعين يحدث في مقدار ثابت واحد"
type: docs
weight: 260
url: /ar/net/aspose.tasks/asn/fixedmaterial/
---
## Asn.FixedMaterial field

يحدد ما إذا كان استهلاك المورد المادي المخصص يحدث بمقدار ثابت واحد.

```csharp
public static readonly Key<bool, AsnKey> FixedMaterial;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Asn.FixedMaterial.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.FixedMaterial, true);

Console.WriteLine("Fixed Material: " + assignment.Get(Asn.FixedMaterial));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


