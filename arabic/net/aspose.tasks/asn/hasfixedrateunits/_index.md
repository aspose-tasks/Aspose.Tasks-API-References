---
title: "Asn.HasFixedRateUnits"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. يحدد ما إذا كانت الوحدات ذات معدل ثابت"
type: docs
weight: 270
url: /ar/net/aspose.tasks/asn/hasfixedrateunits/
---
## Asn.HasFixedRateUnits field

يحدد ما إذا كانت الوحدات لها معدل ثابت.

```csharp
public static readonly Key<bool, AsnKey> HasFixedRateUnits;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Asn.HasFixedRateUnits.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.HasFixedRateUnits, true);

Console.WriteLine("Has Fixed Rate Units: " + assignment.Get(Asn.HasFixedRateUnits));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


