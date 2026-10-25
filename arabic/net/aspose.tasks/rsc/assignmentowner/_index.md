---
title: "Rsc.AssignmentOwner"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. اسم مالك المهمة"
type: docs
weight: 100
url: /ar/net/aspose.tasks/rsc/assignmentowner/
---
## Rsc.AssignmentOwner field

اسم مالك التعيين.

```csharp
public static readonly Key<string, RscKey> AssignmentOwner;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Rsc.AssignmentOwner.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwner, "John");

Console.WriteLine("Assignment Owner: " + resource.Get(Rsc.AssignmentOwner));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


